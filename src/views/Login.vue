<template>
  <div class="home">
    <body class="" id="body">
    <div class="container d-flex align-items-center justify-content-center vh-100">
      <div class="row justify-content-center">
        <div class="col-lg-6 col-md-10">
          <div class="card">
            <div class="card-header bg-primary">
              <div class="app-brand">
                <a href="/index.html">
                  <svg class="brand-icon" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid" width="30" height="33"
                    viewBox="0 0 30 33">
                    <g fill="none" fill-rule="evenodd">
                      <path class="logo-fill-blue" fill="#7DBCFF" d="M0 4v25l8 4V0zM22 4v25l8 4V0z" />
                      <path class="logo-fill-white" fill="#FFF" d="M11 4v25l8 4V0z" />
                    </g>
                  </svg>
                  <span class="brand-name">Dealership Login</span>
                </a>
              </div>
            </div>
            <div class="card-body p-5">
              <h4 class="text-dark mb-5">Sign In</h4>
              <form v-on:submit.prevent="submit()">
                <div class="row">
                  <div class="form-group col-md-12 mb-4">
                    <input type="email" class="form-control input-lg" id="email" aria-describedby="emailHelp" placeholder="Email" v-model="email">
                  </div>
                  <div class="form-group col-md-12 ">
                    <input type="password" class="form-control input-lg" id="password" placeholder="Password" v-model="password">
                  </div>
                  <div class="col-md-12">
                    <div class="d-flex my-2 justify-content-between">
                      <div class="d-inline-block mr-3">
                        <label class="control control-checkbox">Remember me
                          <input type="checkbox" />
                          <div class="control-indicator"></div>
                        </label>
                      </div>
                    </div>
                    <button type="submit" class="btn btn-lg btn-primary btn-block mb-4">Sign In</button>
                    <p>Don't have an account yet ?
                      <a class="text-blue" href="sign-up.html">Try These</a>
                    </p>
                    <div class="row">
                      <div class="col-md col-lg col-xl">
                        <div class="media widget-media p-4 bg-white border">
                          <div class="icon rounded-circle mr-4 bg-primary">
                            <i class="mdi mdi-account-outline text-white "></i>
                          </div>

                          <div class="media-body align-self-center">
                            <h4 class="text-primary mb-2">bob@samos.com</h4>
                            <p>password</p>
                          </div>
                        </div>
                      </div>
                    </div>
                    <div class="row">
                      <div class="col-md col-lg col-xl">
                        <div class="media widget-media p-4 bg-white border">
                          <div class="icon rounded-circle mr-4 bg-warning">
                            <i class="mdi mdi-account-outline text-white "></i>
                          </div>

                          <div class="media-body align-self-center">
                            <h4 class="text-warning mb-2">matt@grove.com</h4>
                            <p>password</p>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>


    <!-- <script type="module">
      import 'https://cdn.jsdelivr.net/npm/@pwabuilder/pwaupdate';

      const el = document.createElement('pwa-update');
      document.body.appendChild(el);
    </script> -->

    <!-- Javascript -->
<!--     <script src="/assets/plugins/jquery/jquery.min.js"></script>
    <script src="/assets/plugins/bootstrap/js/bootstrap.bundle.min.js"></script>
    <script src="/assets/js/sleek.js"></script>
  <link href="/assets/options/optionswitch.css" rel="stylesheet">
<script src="/assets/options/optionswitcher.js"></script> -->
</body>
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
      email: "",
      password: "",
      errors: [],
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
      console.log("Logging in...", this.email, this.password);
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
          if (this.email == "manu@facturer.com") {
            this.$router.push("/manufacturer");}
          else {
            this.$router.push("/");
          }
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