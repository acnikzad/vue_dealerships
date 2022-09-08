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
          
          
          <div class="row">
            <div class="col-md-6 col-lg-6 col-xl-3">
              <div class="media widget-media p-4 bg-white border">
                <div class="icon rounded-circle mr-4 bg-primary">
                  <i class="mdi mdi-account-outline text-white "></i>
                </div>

                <div class="media-body align-self-center">
                  <h4 class="text-primary mb-2">This is Manufacturer</h4>
                  <!-- <p>{{dealer.car.count}}</p> -->
                </div>
              </div>
            </div>
          </div>
          <div class="content-wrapper">
            <div class="content">
              <!--   <div>
                  <h3>Search for cars here:</h3><input type="text" v-model="searchTerm" list="models">
                  <datalist id="titles">
                    <option v-for="car in cars">{{ car.model }}</option>
                  </datalist>
                </div> -->
 <!--                <transition-group appear enter-active-class="animated fadeIn" leave-active-class="animated fadeOut">
                  <div v-for="car in orderBy(filterBy(cars, searchTerm, 'makes', 'models'), sortAttribute, sortOrder)" v-bind:class="{selected: car.selected}" v-bind:key="car.id">
                    <button v-on:click="selectCar(car)">Select Car</button>
                    <p>id: {{ car.id }}</p>
                    <p>Make: {{ car.make }}</p>
                    <p>Model: {{ car.model }}</p>
                    <p>Drivetrain: {{ car.drivetrain }}</p>
                    <br>

                    <button v-on:click="toggleInfo(car)">See more info</button>

                    <div v-if="currentCar === car">
                      <p>prep_time: {{ car.prep_time }}</p>
                      <p>directions: {{ car.directions }}</p>

                      <p>Title: <input type="text" v-model="car.title"></p>
                      <p>Ingredients: <input type="text" v-model="car.ingredients"></p>
                      <p>Directions: <input type="text" v-model="car.directions"></p>
                      <p>Prep Time: <input type="text" v-model="car.prep_time"></p>
                      <p>Chef: <input type="text" v-model="car.chef"></p>
                      <button v-on:click="updateCar(car)">Update the Car</button>
                      <button v-on:click="destroyCar(car)">Destroy Car</button>
                    </div>
                    <hr>
                  </div>
                </transition-group> -->

                <div class="row">
                  <div class="col-12">
                    <div class="card card-default">
                      <div class="card-header card-header-border-bottom d-flex justify-content-between">
                        <h2>Inventory</h2>
                      </div>
                      <div class="row justify-content-between top-information">
                        <div class="dataTables_length" id="basic-data-table_length">
                          <label>Show <select name="basic-data-table_length" aria-controls="basic-data-table" class="custom-select custom-select-sm form-control form-control-sm">
                            <option value="10">10</option>
                            <option value="25">25</option>
                            <option value="50">50</option>
                            <option value="100">100</option>
                          </select> entries</label>
                        </div>
                        <div id="basic-data-table_filter" class="dataTables_filter">
                          <label>Search:<input type="search" class="form-control form-control-sm" placeholder="" aria-controls="basic-data-table"></label>
                        </div>
                      </div>
<!--                        <table id="basic-data-table" class="table nowrap" style="width:100%">
                        <thead>
                         <tr>
                          <th>First name</th>
                          <th>Last name</th>
                          <th>Position</th>
                          <th>Office</th>
                          <th>Age</th>
                          <th>Start date</th>
                          <th>Salary</th>
                          <th>Extn.</th>
                          <th>E-mail</th>
                         </tr>
                        </thead>

                        <tbody>
                         <tr>
                          <td>Tiger</td>
                          <td>Nixon</td>
                          <td>System Architect</td>
                          <td>Edinburgh</td>
                          <td>61</td>
                          <td>2011/04/25</td>
                          <td>$320,800</td>
                          <td>5421</td>
                          <td>t.nixon@datatables.net</td>
                         </tr>
                        </tbody>
                       </table> -->
                      <div class="card-body">
                        <div class="hoverable-data-table">
                          <table id="hoverable-data-table" class="table table-hover nowrap" style="width:100%">
                            <thead>
                              <tr>
                                <th>Year</th>
                                <th>Make</th>
                                <th>Model</th>
                                <th>Color</th>
                                <th>Drivetrain</th>
                                <th>Type</th>
                                <th>Mileage</th>
                                <th>Price</th>
                                <th>Dealership</th>
                                <th>Sell</th>
                              </tr>
                            </thead>
                            <tbody>
                              <tr v-for="car in inventory">
                                <td>{{car.year}}</td>
                                <td>{{car.make}}</td>
                                <td>{{car.model}}</td>
                                <td>{{car.color}}</td>
                                <td>{{car.drivetrain}}</td>
                                <td>{{car.car_type}}</td>
                                <td>{{car.mileage}}</td>
                                <td>{{car.price}}</td>
                                <td>{{car.dealer.name}}</td>
                                <td><button type="button" class="mb-1 btn btn-sm btn-outline-success" data-toggle="modal" data-target="#exampleModal">Sell</button></td>
                              </tr>
                            </tbody>
                          </table>
                        </div>
                      </div>
                      <div class="modal fade" id="exampleModal" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true">
                        <div class="modal-dialog" role="document">
                          <div class="modal-content">
                            <div class="modal-header">
                              <h5 class="modal-title" id="exampleModalLabel">Sell Car</h5>
                              <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                                <span aria-hidden="true">&times;</span>
                              </button>
                            </div>

                            <div class="modal-body">
                              Modal body text goes here.
                            </div>

                            <div class="modal-footer">
                              <button type="button" class="btn btn-outline-danger btn-pill" data-dismiss="modal">Cancel</button>
                              <button type="button" class="btn btn-outline-success btn-pill">Sell Car</button>
                            </div>
                          </div>
                        </div>
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
      sortOrder: 1
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
    axios.get("/api/cars/inventory").then(response => {
      this.inventory = response.data;
      console.log("Current Inventory...", this.inventory)
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


  }
};
</script>