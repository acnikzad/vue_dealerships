<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <button v-on:click="login()">Login</button>
    <!-- The Compound Interest Modal-->
    <div class="modal fade" id="login" tabindex="-1" role="dialog" aria-labelledby="myModalLabel" aria-hidden="true">
      <div class="modal-dialog modal-lg">
        <div class="modal-content">
          <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-hidden="true">
              <i class="tim-icons icon-simple-remove"></i>
            </button>
            <h5 class="modal-title" id="myModalLabel">Login</h5>
          </div>
          <div class="modal-body">
            <div class="col-md-12">
              <div class="card">
                <div class="card-header">
                  <h4 class="card-title">Enter Credentials</h4>
                </div>
                <div class="card-body">
                  <form id="RangeValidation" class="form-horizontal">
                    <div class="row">
                      <label class="col-sm-2 col-form-label">Email:</label>
                      <div class="col-sm-10">
                        <div class="form-group">
                          <input class="form-control" type="text" v-model="email">
                        </div>
                      </div>
                    </div>
                    <div class="row">
                      <label class="col-sm-2 col-form-label">Password:</label>
                      <div class="col-sm-10">
                        <div class="form-group">
                          <input type="password" class="form-control" v-model="password">
                          <p>Email: bob@samos.com</p>
                          <p>Password: password</p>
                        </div>
                      </div>
                    </div>
                  </form>
                </div>
              </div>
            </div>
          </div>
          <div class="modal-footer justify-content-center">
            <button class="btn btn-primary animation-on-hover" rel="tooltip" data-original-title="To the moon!" data-placement="bottom" data-dismiss="modal" v-on:click="ci_account(), resumeClock(), startTimer()">Login</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
</style>

<script>

import axios from "axios";

export default {
  data: function() {
    return {
      users: [],
      dealers: [],
      cars: [],
    };
  },
  created: function() {
    axios.get("/api/users").then(response => {
      this.users = response.data;
      console.log(this.users)
    });
    axios.get("/api/dealers").then(response => {
      this.dealers = response.data;
      console.log(this.dealers)
    });
    axios.get("/api/cars").then(response => {
      this.cars = response.data;
      console.log(this.cars)
    });


  },
  methods: {

    login(){
        console.log("Logging in...");
        $('#login').modal({backdrop: 'static', keyboard: false}, 'show');
      },
    submit: function() {
      var params = {
        email: this.email,
        password: this.password
      };
      axios
        .post("/api/sessions", params)
        .then(response => {
          axios.defaults.headers.common["Authorization"] =
            "Bearer " + response.data.jwt;
          localStorage.setItem("jwt", response.data.jwt);
          this.$router.push("/profile");
        })
        .catch(error => {
          this.errors = ["Invalid email or password"];
          this.email = "";
          this.password = "";
        });
    }


  }
};
</script>