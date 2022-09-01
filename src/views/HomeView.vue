<template>
  <div class="home">
    <h1>{{ message }}</h1>
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
  methods: {}
};
</script>