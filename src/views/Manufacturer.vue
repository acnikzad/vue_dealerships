<template>
  <div class="home">
      <!-- ====================================
    ——— WRAPPER
    ===================================== -->
    <div class="wrapper">

      <!-- Github Link -->
      <a href="https://github.com/tafcoder/sleek-dashboard"  target="_blank" class="github-link">
        <svg width="70" height="70" viewBox="0 0 250 250" aria-hidden="true">
          <defs>
            <linearGradient id="grad1" x1="0%" y1="75%" x2="100%" y2="0%">
              <stop offset="0%" style="stop-color:#896def;stop-opacity:1" />
              <stop offset="100%" style="stop-color:#482271;stop-opacity:1" />
            </linearGradient>
          </defs>
          <path d="M 0,0 L115,115 L115,115 L142,142 L250,250 L250,0 Z" fill="url(#grad1)"></path>
        </svg>
        <i class="mdi mdi-github-circle"></i>
      </a>
<!-- ====================================
——— LEFT SIDEBAR WITH OUT FOOTER
===================================== -->
        <aside class="left-sidebar bg-sidebar">
          <div id="sidebar" class="sidebar sidebar-with-footer">
            <!-- Aplication Brand -->
            <div class="app-brand">
              <a href="/index.html" title="Sleek Dashboard">
                <svg
                  class="brand-icon"
                  xmlns="http://www.w3.org/2000/svg"
                  preserveAspectRatio="xMidYMid"
                  width="30"
                  height="33"
                  viewBox="0 0 30 33">
                  <g fill="none" fill-rule="evenodd">
                    <path class="logo-fill-blue" fill="#7DBCFF" d="M0 4v25l8 4V0zM22 4v25l8 4V0z" />
                    <path class="logo-fill-white" fill="#FFF" d="M11 4v25l8 4V0z" />
                  </g>
                </svg>

                <span class="brand-name text-truncate">Sleek Dashboard</span>
              </a>
            </div>

            <!-- begin sidebar scrollbar -->
            <div class="" data-simplebar style="height: 100%;">
              <!-- sidebar menu -->
              <ul class="nav sidebar-inner" id="sidebar-menu">
                <li class="has-sub ">
                  <a class="sidenav-item-link" href="javascript:void(0)" data-toggle="collapse" data-target="#dashboard"
                    aria-expanded="false" aria-controls="dashboard">
                    <i class="mdi mdi-view-dashboard-outline"></i>
                    <span class="nav-text">Dashboard</span> <b class="caret"></b>
                  </a>

                  <ul class="collapse " id="dashboard" data-parent="#sidebar-menu">
                    <div class="sub-menu">
                      <li class="">
                        <a class="sidenav-item-link" href="index.html">
                          <span class="nav-text">Ecommerce</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="analytics.html">
                          <span class="nav-text">Analytics</span>
                          <span class="badge badge-success">new</span>
                        </a>
                      </li>
                    </div>
                  </ul>
                </li>

                <li class="has-sub ">
                  <a class="sidenav-item-link" href="javascript:void(0)" data-toggle="collapse" data-target="#app"
                    aria-expanded="false" aria-controls="app">
                    <i class="mdi mdi-pencil-box-multiple"></i>
                    <span class="nav-text">App</span> <b class="caret"></b>
                  </a>

                  <ul class="collapse " id="app" data-parent="#sidebar-menu">
                    <div class="sub-menu">
                      <li class="">
                        <a class="sidenav-item-link" href="chat.html">
                          <span class="nav-text">Chat</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="contacts.html">
                          <span class="nav-text">Contacts</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="team.html">
                          <span class="nav-text">Team</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="calendar.html">
                          <span class="nav-text">Calendar</span>
                        </a>
                      </li>
                    </div>
                  </ul>
                </li>

                <!-- <li class="section-title">
                  UI Elements
                </li> -->

                <li class="has-sub ">
                  <a class="sidenav-item-link" href="javascript:void(0)" data-toggle="collapse" data-target="#components"
                    aria-expanded="false" aria-controls="components">
                    <i class="mdi mdi-folder-multiple-outline"></i>
                    <span class="nav-text">Components</span> <b class="caret"></b>
                  </a>

                  <ul class="collapse " id="components" data-parent="#sidebar-menu">
                    <div class="sub-menu">
                      <li class="">
                        <a class="sidenav-item-link" href="alert.html">
                          <span class="nav-text">Alert</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="badge.html">
                          <span class="nav-text">Badge</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="breadcrumb.html">
                          <span class="nav-text">Breadcrumb</span>

                        </a>
                      </li>

                      <li class="has-sub ">
                        <a class="sidenav-item-link" href="javascript:void(0)" data-toggle="collapse" data-target="#buttons"
                          aria-expanded="false" aria-controls="buttons">
                          <span class="nav-text">Buttons</span> <b class="caret"></b>
                        </a>

                        <ul class="collapse " id="buttons">
                          <div class="sub-menu">
                            <li class="">
                              <a href="button-default.html">Button Default</a>
                            </li>

                           <li class="">
                              <a href="button-dropdown.html">Button Dropdown</a>
                            </li>

                           <li class="">
                              <a href="button-group.html">Button Group</a>
                            </li>

                           <li class="">
                              <a href="button-social.html">Button Social</a>
                            </li>

                           <li class="">
                              <a href="button-loading.html">Button Loading</a>
                            </li>
                          </div>
                        </ul>
                      </li>
                      
                      <li class="">
                        <a class="sidenav-item-link" href="card.html">
                          <span class="nav-text">Card</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="carousel.html">
                          <span class="nav-text">Carousel</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="collapse.html">
                          <span class="nav-text">Collapse</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="list-group.html">
                          <span class="nav-text">List Group</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="modal.html">
                          <span class="nav-text">Modal</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="pagination.html">
                          <span class="nav-text">Pagination</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="popover-tooltip.html">
                          <span class="nav-text">Popover & Tooltip</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="progress-bar.html">
                          <span class="nav-text">Progress Bar</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="spinner.html">
                          <span class="nav-text">Spinner</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="switcher.html">
                          <span class="nav-text">Switcher</span>
                        </a>
                      </li>

                      <li class="">
                        <a class="sidenav-item-link" href="tab.html">
                          <span class="nav-text">Tab</span>
                        </a>
                      </li>
                    </div>
                  </ul>
                </li>
              </ul>
            </div>
          </div>
        </aside>


          <!-- ====================================
        ——— PAGE WRAPPER
        ===================================== -->
        <div class="page-wrapper">
          <!-- Header -->
          <header class="main-header " id="header">
            <nav class="navbar navbar-static-top navbar-expand-lg">
              <!-- Sidebar toggle button -->
              <button id="sidebar-toggler" class="sidebar-toggle">
                <span class="sr-only">Toggle navigation</span>
              </button>
              <!-- search form -->
              <div class="search-form d-none d-lg-inline-block">
                <div class="input-group">
                  <button type="button" name="search" id="search-btn" class="btn btn-flat">
                    <i class="mdi mdi-magnify"></i>
                  </button>
                  <input type="text" name="query" id="search-input" class="form-control" placeholder="'button', 'chart' etc."
                    autofocus autocomplete="off" />
                </div>
                <div id="search-results-container">
                  <ul id="search-results"></ul>
                </div>
              </div>
            </nav>
          </header>
          <div class="content-wrapper">
            <div class="content">

              <div class="breadcrumb-wrapper">
                <h1>Manufacturer</h1>
              </div>
              <div class="row">
                <div class="col-lg-6">
                  <div class="card card-default">
                    <div class="card-header card-header-border-bottom">
                      <h2>Create Car</h2>
                    </div>

                    <div class="card-body">
                      <form id="createCar">
                        <div class="form-group">
                          <label>Year</label>
                          <input type="number" class="form-control input-sm" id="year" placeholder="2015" v-model="year">
                        </div>
                        <div class="form-group">
                          <label>Make</label>
                          <select class="form-control input-sm" v-model="make">
                            <option value="" disabled selected>Select Make</option>
                            <option>Acura</option>
                            <option>Audi</option>
                            <option>BMW</option>
                            <option>Cheverolet</option>
                            <option>Dodge</option>
                            <option>Ford</option>
                            <option>Honda</option>
                            <option>Lexus</option>
                            <option>Mazda</option>
                            <option>Mercedes-Benz</option>
                            <option>Mini</option>
                            <option>Nissan</option>
                            <option>Subaru</option>
                            <option>Toyota</option>
                            <option>Volkswagon</option>
                          </select>
                        </div>
                        <div class="form-group">
                          <label for="exampleFormControlInput1">Model</label>
                          <input type="text" class="form-control input-sm" id="year" placeholder="Accord" v-model="model">
                        </div>
                     <!--    <div class="form-group">
                          <label for="exampleFormControlPassword">Model</label>
                          <select class="form-control input-sm" v-model="carModel">
                            <option>Acura</option>
                            <option>BMW</option>
                            <option>Cheverolet</option>
                            <option>Dodge</option>
                            <option>Ford</option>
                            <option>Honda</option>
                            <option>Nissan</option>
                            <option>Subaru</option>
                            <option>Toyota</option>
                            <option>Volkswagon</option>
                          </select>
                        </div> -->
                        <div class="form-group">
                          <label for="exampleFormControlSelect12">Color</label>
                          <select class="form-control input-sm" id="exampleFormControlSelect12" v-model="color">
                            <option value="" disabled selected>Select Color</option>
                            <option>Blue</option>
                            <option>Black</option>
                            <option>White</option>
                            <option>Silver</option>
                            <option>Red</option>
                            <option>Green</option>
                            <option>Charcoal</option>
                          </select>
                        </div>
                        <div class="form-group row">
                          <div class="col-12 col-md-3 text-right">
                            <label for="Radios">Drivetrain</label>
                          </div>
                          <div class="col-12 col-md-9">
                            <label class="control control-radio">FWD
                              <input type="radio" name="FWD" v-model="drivetrain" value="FWD"/>
                              <div class="control-indicator"></div>
                            </label>

                            <label class="control control-radio">RWD
                              <input type="radio" name="RWD" v-model="drivetrain" value="RWD"/>
                              <div class="control-indicator"></div>
                            </label>

                            <label class="control control-radio">4x4
                              <input type="radio" name="4x4" v-model="drivetrain" value="4x4"/>
                              <div class="control-indicator"></div>
                            </label>
                            <label class="control control-radio">AWD
                              <input type="radio" name="AWD" v-model="drivetrain" value="AWD"/>
                              <div class="control-indicator"></div>
                            </label>
                          </div>
                        </div>
                        <div class="form-group">
                          <label for="exampleFormControlSelect12">Car Type</label>
                          <select class="form-control input-sm" id="exampleFormControlSelect12" v-model="car_type">
                            <option value="" disabled selected>Select Car Type</option>
                            <option>Sedan</option>
                            <option>Coupe</option>
                            <option>SUV</option>
                            <option>Truck</option>
                            <option>Hatchback</option>
                            <option>Crossover</option>
                            <option>Wagon</option>
                          </select>
                        </div>
                        <div class="form-group">
                          <label for="exampleFormControlInput1">Mileage</label>
                          <input type="number" class="form-control input-sm" id="mileage" placeholder="23,673" v-model="mileage">
                        </div>
                        <div class="form-group">
                          <label for="exampleFormControlInput1">Price</label>
                          <input type="number" class="form-control input-sm" id="price" placeholder="$7,999" v-model="price">
                        </div>
                        <div class="form-group">
                          <label for="exampleFormControlSelect12">Assign to Location</label>
                          <select class="form-control input-sm" id="" v-model="dealer_id">
                            <option v-for="dealer in dealers" :value="dealer.id">{{dealer.name}} - {{dealer.city}}</option>
                          </select>
                        </div>
                        <div class="form-footer pt-4 pt-5 mt-4 border-top">
                          <button type="submit" class="btn btn-primary btn-default" v-on:click="createCar()">Submit</button>
                        </div>
                      </form>
                    </div>
                  </div>
                </div>
                <div class="col-lg-6">
                  <div class="card card-default">
                    <div class="card-header card-header-border-bottom">
                      <h2>Create User</h2>
                    </div>

                    <div class="card-body">
                      <form name ="userCreate" @submit.prevent="userCreate">
                        <div class="form-group">
                          <label for="exampleFormControlInput1">First Name</label>
                          <input type="text" class="form-control input-sm" id="exampleFormControlInput1" placeholder="Aria" v-model="first_name">
                        </div>

                        <div class="form-group">
                          <label for="exampleFormControlPassword">Last Name</label>
                          <input type="text" class="form-control" id="exampleFormControlPassword" placeholder="Nikzad" v-model="last_name">
                        </div>

                        <div class="form-footer pt-4 pt-5 mt-4 border-top">
                          <button type="submit" class="btn btn-primary btn-default" v-on:click="createUser()">Submit</button>
                        </div>
                      </form>
                    </div>
                  </div>

                  <div class="card card-default">
                    <div class="card-header card-header-border-bottom">
                      <h2>Create Dealership</h2>
                    </div>

                    <div class="card-body">
                      <form>
                        <div class="form-group">
                          <label for="exampleFormControlInput1">Dealer Name</label>
                          <input type="text" class="form-control input-sm" id="exampleFormControlInput1" placeholder="Arias Rad Rides" v-model="dealer_name">
                        </div>

                        <div class="form-group">
                          <label for="exampleFormControlPassword">Phone Number</label>
                          <input type="text" class="form-control" id="exampleFormControlPassword" placeholder="(111) 111-1111" v-model="phone">
                        </div>

                        <div class="form-group">
                          <label for="exampleFormControlPassword">Street Address</label>
                          <input type="text" class="form-control" id="exampleFormControlPassword" placeholder="123 1st Street" v-model="address">
                        </div>

                        <div class="form-group">
                          <label for="exampleFormControlPassword">City</label>
                          <input type="text" class="form-control" id="exampleFormControlPassword" placeholder="Sacramento" v-model="city">
                        </div>

                         <div class="form-group">
                          <label for="exampleFormControlPassword">Cash On Hand</label>
                          <input type="number" class="form-control" id="exampleFormControlPassword" placeholder="40000" v-model="cash">
                        </div>

                        <div class="form-group">
                          <label for="exampleFormControlSelect12">Dealer Manager</label>
                          <select class="form-control input-sm" id="" v-model="user_id">
                            <option v-for="user in users" :value="user.id">{{user.first_name}} {{user.last_name}}</option>
                          </select>
                        </div>

                        <div class="form-footer pt-4 pt-5 mt-4 border-top">
                          <button type="submit" class="btn btn-primary btn-default" v-on:click="createDealer()">Submit</button>
                        </div>
                      </form>
                    </div>
                  </div>
                </div>
              </div>

              </div> <!-- End Content -->
            </div> <!-- End Content Wrapper -->
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
      inventory: [],
      email: "",
      password: "",
      searchTerm: "",
      currentCar: {},
      sortAttribute: 'make',
      sortOrder: 1,

      year: "",
      make: "",
      model: "",
      color: "",
      drivetrain: "",
      car_type: "",
      mileage: "",
      price: "",
      dealer_id: "",

      first_name: "",
      last_name: "",
      email: "",
      password: "",

      dealer_name: "",
      phone: "",
      address: "",
      city: "",
      cash: "",
      user_id: ""

    };
  },
  created: function() {
    axios.get("/api/users").then(response => {
      this.users = response.data;
      console.log("Users...", this.users)
    });
    axios.get("/api/dealers").then(response => {
      this.dealers = response.data;
      console.log("Dealers...", this.dealers)
    });
    axios.get("/api/cars").then(response => {
      this.cars = response.data;
      console.log("Cars...", this.cars)
    });
    // axios.get("/api/cars/inventory").then(response => {
    //   this.inventory = response.data;
    //   console.log("Current Inventory...", this.inventory)
    // });

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
          this.$router.push("/HomeView");
        })
        .catch(error => {
          this.errors = ["Invalid email or password"];
          this.email = "";
          this.password = "";
        });
    },

    selectCar: function(theCar) {
      console.log('selecting the car');
      theCar.selected = !theCar.selected;
      console.log(theCar);
    },

    toggleInfo: function(theCar) {
      console.log(theCar);
      if (this.currentCar === theCar) {
        this.currentCar = null;
      } else {
        this.currentCar = theCar;
      }
      console.log('in toggle info...');
    },

    setSortAttribute: function(theAttribute) {
      this.sortAttribute = theAttribute;
      // this.sortOrder = -1;
      console.log(this.sortOrder === 1);
      if (this.sortOrder === 1) {
        this.sortOrder = -1;
      } else {
        this.sortOrder = 1;
      }
    },

    // createStudent: function() {
    //   console.log("creating student...")
    //   let params = {
    //         first_name: this.newStudentFirstName,
    //         last_name: this.newStudentLastName
    //   };
    //   axios.post("/api/students", params).then(response => {
    //     this.students.push(response.data);
    //     this.newStudentFirstName = "";
    //     this.newStudentLastName = "";
    //   })
    // },
    createCar: function() {
      let params = {
            year: this.year,
            make: this.make,
            model: this.model,
            color: this.color,
            drivetrain: this.drivetrain,
            car_type: this.car_type,
            mileage: this.mileage,
            price: this.price,
            dealer_id: this.dealer_id
      };
      console.log(params)
      axios.post("/api/cars", params).then(response => {
        console.log("this is the response data", response.data)
        this.cars.push(response.data);
        this.year = "";
        this.make = "";
        this.model = "";
        this.color = "";
        this.drivetrain = "";
        this.car_type = "";
        this.mileage = "";
        this.price = "";
        this.dealer_id = "";
        })
    },

    createUser: function() {
      console.log("creating")
      this.email = this.first_name.toLowerCase()+"@"+this.last_name.toLowerCase()+".com"
      let params = {
            first_name: this.first_name,
            last_name: this.last_name,
            email: this.email,
            password: "password"
      };
      console.log(params)
      axios.post("/api/users", params).then(response => {
        console.log("this is the response data", response.data)
        this.users.push(response.data);
        this.first_name = "";
        this.last_name = "";
        this.email = "";
        this.password = "";
        })
    },

    createDealer: function() {
      let params = {
            name: this.dealer_name,
            phone: this.phone,
            address: this.address,
            city: this.city,
            cash: this.cash,
            user_id: this.user_id,
            password: "password"
      };
      console.log(params)
      axios.post("/api/dealers", params).then(response => {
        console.log("this is the response data", response.data)
        this.dealers.push(response.data);
        this.dealer_name = "";
        this.phone = "";
        this.address = "";
        this.city = "";
        this.cash = "";
        this.user_id = "";
        })
    },
  }
};
</script>