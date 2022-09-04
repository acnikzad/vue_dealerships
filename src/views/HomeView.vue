<template>
  <div class="home">
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
          </div>              </div>

        <div class="navbar-right ">
          <ul class="nav navbar-nav">
            <li class="dropdown notifications-menu custom-dropdown">
              <button class="dropdown-toggle notify-toggler custom-dropdown-toggler">
                <i class="mdi mdi-bell-outline"></i>
              </button>

              <div class="card card-default dropdown-notify dropdown-menu-right mb-0">
                <div class="card-header card-header-border-bottom px-3">
                  <h2>Notifications</h2>
                </div>

                <div class="card-body px-0 py-3">
                  <ul class="nav nav-tabs nav-style-border p-0 justify-content-between" id="myTab" role="tablist">
                    <li class="nav-item mx-3 my-0 py-0">
                      <a class="nav-link active pb-3" id="home2-tab" data-toggle="tab" href="#home2" role="tab" aria-controls="home2" aria-selected="true">All (11)</a>
                    </li>

                    <li class="nav-item mx-3 my-0 py-0">
                      <a class="nav-link pb-3" id="profile2-tab" data-toggle="tab" href="#profile2" role="tab" aria-controls="profile2" aria-selected="false">Msgs (6)</a>
                    </li>

                    <li class="nav-item mx-3 my-0 py-0">
                      <a class="nav-link pb-3" id="contact2-tab" data-toggle="tab" href="#contact2" role="tab" aria-controls="contact2" aria-selected="false">Others (5)</a>
                    </li>
                  </ul>

                  <div class="tab-content" id="myTabContent3">
                    <div class="tab-pane fade show active" id="home2" role="tabpanel" aria-labelledby="home2-tab">
                      <ul class="list-unstyled" data-simplebar style="height: 360px">
                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">
                            <div class="position-relative mr-3">
                              <img class="rounded-circle" src="assets/img/user/u2.jpg" alt="Image">
                              <span class="status away"></span>
                            </div>
                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Aaren</h4>
                                <p class="last-msg">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nam itaque doloremque odio, eligendi delectus vitae.</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 30 min ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification media-active">
                            <div class="position-relative mr-3">
                              <img class="rounded-circle" src="assets/img/user/u1.jpg" alt="Image">
                              <span class="status active"></span>
                            </div>
                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Abril</h4>
                                <p class="last-msg">Donec mattis augue a nisl consequat, nec imperdiet ex rutrum. Fusce et vehicula enim. Sed in enim eu odio vehic.</p>

                                <span class="font-size-12 font-weight-medium text-white">
                                  <i class="mdi mdi-clock-outline"></i> Just now...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">
                            <div class="position-relative mr-3">
                              <img class="rounded-circle" src="assets/img/user/u5.jpg" alt="Image">
                              <span class="status away"></span>
                            </div>
                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Emma</h4>
                                <p class="last-msg">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nam itaque doloremque odio, eligendi delectus vitae.</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 1 hrs ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification event-active">

                            <div class="d-flex rounded-circle align-items-center justify-content-center mr-3 media-icon iconbox-45 bg-info text-white">
                              <i class="mdi mdi-calendar-check font-size-20"></i>
                            </div>

                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">New event added</h4>
                                <p class="last-msg font-size-14">03/Jan/2020 (1pm - 2pm)</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 10 min ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">

                            <div class="d-flex rounded-circle align-items-center justify-content-center mr-3 media-icon iconbox-45 bg-warning text-white">
                              <i class="mdi mdi-chart-areaspline font-size-20"></i>
                            </div>

                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Sales report</h4>
                                <p class="last-msg font-size-14">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nam itaque doloremque odio, eligendi delectus vitae.</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 1 hrs ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">

                            <div class="d-flex rounded-circle align-items-center justify-content-center mr-3 media-icon iconbox-45 bg-primary text-white">
                              <i class="mdi mdi-account-multiple-check font-size-20"></i>
                            </div>

                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Add request</h4>
                                <p class="last-msg font-size-14">Add Dany Jones as your contact consequat nec imperdiet ex rutrum. Fusce et vehicula enim. Sed in enim.</p>

                                <button type="button" class="my-1 btn btn-sm btn-success">Accept</button>
                                <button type="button" class="my-1 btn btn-sm btn-secondary">Delete</button>

                                <span class="font-size-12 font-weight-medium text-secondary d-block">
                                  <i class="mdi mdi-clock-outline"></i> 5 min ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">

                            <div class="d-flex rounded-circle align-items-center justify-content-center mr-3 media-icon iconbox-45 bg-danger text-white">
                              <i class="mdi mdi-server-network-off font-size-20"></i>
                            </div>

                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Server overloaded</h4>
                                <p class="last-msg font-size-14">Donec mattis augue a nisl consequat, nec imperdiet ex rutrum. Fusce et vehicula enim. Sed in enim eu odio vehic.</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 30 min ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">

                            <div class="d-flex rounded-circle align-items-center justify-content-center mr-3 media-icon iconbox-45 bg-purple text-white">
                              <i class="mdi mdi-playlist-check font-size-20"></i>
                            </div>

                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Task complete</h4>
                                <p class="last-msg font-size-14">Nam ut nisi erat. Ut quis tortor varius, hendrerit arcu quis, congue nisl. In scelerisque, sem ut ve.</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 2 hrs ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                      </ul>
                    </div>

                    <div class="tab-pane fade" id="profile2" role="tabpanel" aria-labelledby="profile2-tab">
                      <ul class="list-unstyled" data-simplebar style="height: 360px">
                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">
                            <div class="position-relative mr-3">
                              <img class="rounded-circle" src="assets/img/user/u6.jpg" alt="Image">
                              <span class="status away"></span>
                            </div>
                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">William</h4>
                                <p class="last-msg">Donec mattis augue a nisl consequat, nec imperdiet ex rutrum. Fusce et vehicula enim. Sed in enim eu odio vehic.</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 1 hrs ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">
                            <div class="position-relative mr-3">
                              <img class="rounded-circle" src="assets/img/user/u7.jpg" alt="Image">
                              <span class="status away"></span>
                            </div>
                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Camble</h4>
                                <p class="last-msg">Nam ut nisi erat. Ut quis tortor varius, hendrerit arcu quis, congue nisl. In scelerisque, sem ut ve.</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 1 hrs ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification media-active">
                            <div class="position-relative mr-3">
                              <img class="rounded-circle" src="assets/img/user/u1.jpg" alt="Image">
                              <span class="status active"></span>
                            </div>
                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Abril</h4>
                                <p class="last-msg">Donec mattis augue a nisl consequat, nec imperdiet ex rutrum. Fusce et vehicula enim. Sed in enim eu odio vehic.</p>

                                <span class="font-size-12 font-weight-medium text-white">
                                  <i class="mdi mdi-clock-outline"></i> Just now...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">
                            <div class="position-relative mr-3">
                              <img class="rounded-circle" src="assets/img/user/u2.jpg" alt="Image">
                              <span class="status away"></span>
                            </div>
                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Aaren</h4>
                                <p class="last-msg">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nam itaque doloremque odio, eligendi delectus vitae.</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 1 hrs ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">
                            <div class="position-relative mr-3">
                              <img class="rounded-circle" src="assets/img/user/u5.jpg" alt="Image">
                              <span class="status away"></span>
                            </div>
                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Emma</h4>
                                <p class="last-msg">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nam itaque doloremque odio, eligendi delectus vitae.</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 1 hrs ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                      </ul>
                    </div>

                    <div class="tab-pane fade" id="contact2" role="tabpanel" aria-labelledby="contact2-tab">
                      <ul class="list-unstyled" data-simplebar style="height: 360px">
                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification event-active">

                            <div class="d-flex rounded-circle align-items-center justify-content-center mr-3 media-icon iconbox-45 bg-info text-white">
                              <i class="mdi mdi-calendar-check font-size-20"></i>
                            </div>

                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">New event added</h4>
                                <p class="last-msg font-size-14">03/Jan/2020 (1pm - 2pm)</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 10 min ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">

                            <div class="d-flex rounded-circle align-items-center justify-content-center mr-3 media-icon iconbox-45 bg-warning text-white">
                              <i class="mdi mdi-chart-areaspline font-size-20"></i>
                            </div>

                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Sales report</h4>
                                <p class="last-msg font-size-14">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nam itaque doloremque odio, eligendi delectus vitae.</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 1 hrs ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">

                            <div class="d-flex rounded-circle align-items-center justify-content-center mr-3 media-icon iconbox-45 bg-primary text-white">
                              <i class="mdi mdi-account-multiple-check font-size-20"></i>
                            </div>

                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Add request</h4>
                                <p class="last-msg font-size-14">Add Dany Jones as your contact consequat nec imperdiet ex rutrum. Fusce et vehicula enim. Sed in enim.</p>

                                <button type="button" class="my-1 btn btn-sm btn-success">Accept</button>
                                <button type="button" class="my-1 btn btn-sm btn-secondary">Delete</button>

                                <span class="font-size-12 font-weight-medium text-secondary d-block">
                                  <i class="mdi mdi-clock-outline"></i> 5 min ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">

                            <div class="d-flex rounded-circle align-items-center justify-content-center mr-3 media-icon iconbox-45 bg-danger text-white">
                              <i class="mdi mdi-server-network-off font-size-20"></i>
                            </div>

                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Server overloaded</h4>
                                <p class="last-msg font-size-14">Donec mattis augue a nisl consequat, nec imperdiet ex rutrum. Fusce et vehicula enim. Sed in enim eu odio vehic.</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 30 min ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>

                        <li>
                          <a href="javscript:void(0)" class="media media-message media-notification">

                            <div class="d-flex rounded-circle align-items-center justify-content-center mr-3 media-icon iconbox-45 bg-purple text-white">
                              <i class="mdi mdi-playlist-check font-size-20"></i>
                            </div>

                            <div class="media-body d-flex justify-content-between">
                              <div class="message-contents">
                                <h4 class="title">Task complete</h4>
                                <p class="last-msg font-size-14">Nam ut nisi erat. Ut quis tortor varius, hendrerit arcu quis, congue nisl. In scelerisque, sem ut ve.</p>

                                <span class="font-size-12 font-weight-medium text-secondary">
                                  <i class="mdi mdi-clock-outline"></i> 2 hrs ago...
                                </span>
                              </div>
                            </div>
                          </a>
                        </li>
                      </ul>
                    </div>
                  </div>
                </div>
              </div>

              <ul class="dropdown-menu dropdown-menu-right d-none">
                <li class="dropdown-header">You have 5 notifications</li>
                <li>
                  <a href="#">
                    <i class="mdi mdi-account-plus"></i> New user registered
                    <span class=" font-size-12 d-inline-block float-right"><i class="mdi mdi-clock-outline"></i> 10 AM</span>
                  </a>
                </li>
                <li>
                  <a href="#">
                    <i class="mdi mdi-account-remove"></i> User deleted
                    <span class=" font-size-12 d-inline-block float-right"><i class="mdi mdi-clock-outline"></i> 07 AM</span>
                  </a>
                </li>
                <li>
                  <a href="#">
                    <i class="mdi mdi-chart-areaspline"></i> Sales report is ready
                    <span class=" font-size-12 d-inline-block float-right"><i class="mdi mdi-clock-outline"></i> 12 PM</span>
                  </a>
                </li>
                <li>
                  <a href="#">
                    <i class="mdi mdi-account-supervisor"></i> New client
                    <span class=" font-size-12 d-inline-block float-right"><i class="mdi mdi-clock-outline"></i> 10 AM</span>
                  </a>
                </li>
                <li>
                  <a href="#">
                    <i class="mdi mdi-server-network-off"></i> Server overloaded
                    <span class=" font-size-12 d-inline-block float-right"><i class="mdi mdi-clock-outline"></i> 05 AM</span>
                  </a>
                </li>
                <li class="dropdown-footer">
                  <a class="text-center" href="#"> View All </a>
                </li>
              </ul>
            </li>
            <li class="right-sidebar-in right-sidebar-2-menu">
              <i class="mdi mdi-settings mdi-spin"></i>
            </li>
            <!-- User Account -->
            <li class="dropdown user-menu">
              <button href="#" class="dropdown-toggle nav-link" data-toggle="dropdown">
                <img src="assets/img/user/user.png" class="user-image" alt="User Image" />
                <span class="d-none d-lg-inline-block">Abdus Salam</span>
              </button>
              <ul class="dropdown-menu dropdown-menu-right">
                å<!-- User image -->
                <li class="dropdown-header">
                  <img src="assets/img/user/user.png" class="img-circle" alt="User Image" />
                  <div class="d-inline-block">
                    Abdus Salam <small class="pt-1">iamabdus@gmail.com</small>
                  </div>
                </li>

                <li>
                  <a href="user-profile.html">
                    <i class="mdi mdi-account"></i> My Profile
                  </a>
                </li>
                <li>
                  <a href="#">
                    <i class="mdi mdi-email"></i> Message
                  </a>
                </li>
                <li>
                  <a href="#"> <i class="mdi mdi-diamond-stone"></i> Projects </a>
                </li>
                <li class="right-sidebar-in">
                  <a href="javascript:0"> <i class="mdi mdi-settings"></i> Setting </a>
                </li>

                <li class="dropdown-footer">
                  <a href="index.html"> <i class="mdi mdi-logout"></i> Log Out </a>
                </li>
              </ul>
            </li>
          </ul>
        </div>
      </nav>
    </header>
    <div class="row">
  <div class="col-12">
    <div class="card card-default">
      <div class="card-header card-header-border-bottom d-flex justify-content-between">
        <h2>Basic Data Table</h2>

        <a href="https://datatables.net/examples/styling/display.html" target="_blank" class="btn btn-outline-primary btn-sm text-uppercase">
          <i class=" mdi mdi-link mr-1"></i> Docs
        </a>
      </div>

      <div class="card-body">
        <div class="basic-data-table">
          <table id="basic-data-table" class="table nowrap" style="width:100%">
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

              <tr>
                <td>Garrett</td>
                <td>Winters</td>
                <td>Accountant</td>
                <td>Tokyo</td>
                <td>63</td>
                <td>2011/07/25</td>
                <td>$170,750</td>
                <td>8422</td>
                <td>g.winters@datatables.net</td>
              </tr>

              <tr>
                <td>Ashton</td>
                <td>Cox</td>
                <td>Junior Technical Author</td>
                <td>San Francisco</td>
                <td>66</td>
                <td>2009/01/12</td>
                <td>$86,000</td>
                <td>1562</td>
                <td>a.cox@datatables.net</td>
              </tr>

              <tr>
                <td>Cedric</td>
                <td>Kelly</td>
                <td>Senior Javascript Developer</td>
                <td>Edinburgh</td>
                <td>22</td>
                <td>2012/03/29</td>
                <td>$433,060</td>
                <td>6224</td>
                <td>c.kelly@datatables.net</td>
              </tr>

              <tr>
                <td>Airi</td>
                <td>Satou</td>
                <td>Accountant</td>
                <td>Tokyo</td>
                <td>33</td>
                <td>2008/11/28</td>
                <td>$162,700</td>
                <td>5407</td>
                <td>a.satou@datatables.net</td>
              </tr>

              <tr>
                <td>Brielle</td>
                <td>Williamson</td>
                <td>Integration Specialist</td>
                <td>New York</td>
                <td>61</td>
                <td>2012/12/02</td>
                <td>$372,000</td>
                <td>4804</td>
                <td>b.williamson@datatables.net</td>
              </tr>

              <tr>
                <td>Herrod</td>
                <td>Chandler</td>
                <td>Sales Assistant</td>
                <td>San Francisco</td>
                <td>59</td>
                <td>2012/08/06</td>
                <td>$137,500</td>
                <td>9608</td>
                <td>h.chandler@datatables.net</td>
              </tr>

              <tr>
                <td>Rhona</td>
                <td>Davidson</td>
                <td>Integration Specialist</td>
                <td>Tokyo</td>
                <td>55</td>
                <td>2010/10/14</td>
                <td>$327,900</td>
                <td>6200</td>
                <td>r.davidson@datatables.net</td>
              </tr>

              <tr>
                <td>Colleen</td>
                <td>Hurst</td>
                <td>Javascript Developer</td>
                <td>San Francisco</td>
                <td>39</td>
                <td>2009/09/15</td>
                <td>$205,500</td>
                <td>2360</td>
                <td>c.hurst@datatables.net</td>
              </tr>

              <tr>
                <td>Sonya</td>
                <td>Frost</td>
                <td>Software Engineer</td>
                <td>Edinburgh</td>
                <td>23</td>
                <td>2008/12/13</td>
                <td>$103,600</td>
                <td>1667</td>
                <td>s.frost@datatables.net</td>
              </tr>

              <tr>
                <td>Jena</td>
                <td>Gaines</td>
                <td>Office Manager</td>
                <td>London</td>
                <td>30</td>
                <td>2008/12/19</td>
                <td>$90,560</td>
                <td>3814</td>
                <td>j.gaines@datatables.net</td>
              </tr>

              <tr>
                <td>Quinn</td>
                <td>Flynn</td>
                <td>Support Lead</td>
                <td>Edinburgh</td>
                <td>22</td>
                <td>2013/03/03</td>
                <td>$342,000</td>
                <td>9497</td>
                <td>q.flynn@datatables.net</td>
              </tr>

              <tr>
                <td>Charde</td>
                <td>Marshall</td>
                <td>Regional Director</td>
                <td>San Francisco</td>
                <td>36</td>
                <td>2008/10/16</td>
                <td>$470,600</td>
                <td>6741</td>
                <td>c.marshall@datatables.net</td>
              </tr>

              <tr>
                <td>Haley</td>
                <td>Kennedy</td>
                <td>Senior Marketing Designer</td>
                <td>London</td>
                <td>43</td>
                <td>2012/12/18</td>
                <td>$313,500</td>
                <td>3597</td>
                <td>h.kennedy@datatables.net</td>
              </tr>

              <tr>
                <td>Tatyana</td>
                <td>Fitzpatrick</td>
                <td>Regional Director</td>
                <td>London</td>
                <td>19</td>
                <td>2010/03/17</td>
                <td>$385,750</td>
                <td>1965</td>
                <td>t.fitzpatrick@datatables.net</td>
              </tr>

              <tr>
                <td>Michael</td>
                <td>Silva</td>
                <td>Marketing Designer</td>
                <td>London</td>
                <td>66</td>
                <td>2012/11/27</td>
                <td>$198,500</td>
                <td>1581</td>
                <td>m.silva@datatables.net</td>
              </tr>

              <tr>
                <td>Paul</td>
                <td>Byrd</td>
                <td>Chief Financial Officer (CFO)</td>
                <td>New York</td>
                <td>64</td>
                <td>2010/06/09</td>
                <td>$725,000</td>
                <td>3059</td>
                <td>p.byrd@datatables.net</td>
              </tr>

              <tr>
                <td>Gloria</td>
                <td>Little</td>
                <td>Systems Administrator</td>
                <td>New York</td>
                <td>59</td>
                <td>2009/04/10</td>
                <td>$237,500</td>
                <td>1721</td>
                <td>g.little@datatables.net</td>
              </tr>

              <tr>
                <td>Bradley</td>
                <td>Greer</td>
                <td>Software Engineer</td>
                <td>London</td>
                <td>41</td>
                <td>2012/10/13</td>
                <td>$132,000</td>
                <td>2558</td>
                <td>b.greer@datatables.net</td>
              </tr>

              <tr>
                <td>Dai</td>
                <td>Rios</td>
                <td>Personnel Lead</td>
                <td>Edinburgh</td>
                <td>35</td>
                <td>2012/09/26</td>
                <td>$217,500</td>
                <td>2290</td>
                <td>d.rios@datatables.net</td>
              </tr>

              <tr>
                <td>Jenette</td>
                <td>Caldwell</td>
                <td>Development Lead</td>
                <td>New York</td>
                <td>30</td>
                <td>2011/09/03</td>
                <td>$345,000</td>
                <td>1937</td>
                <td>j.caldwell@datatables.net</td>
              </tr>

              <tr>
                <td>Yuri</td>
                <td>Berry</td>
                <td>Chief Marketing Officer (CMO)</td>
                <td>New York</td>
                <td>40</td>
                <td>2009/06/25</td>
                <td>$675,000</td>
                <td>6154</td>
                <td>y.berry@datatables.net</td>
              </tr>

              <tr>
                <td>Caesar</td>
                <td>Vance</td>
                <td>Pre-Sales Support</td>
                <td>New York</td>
                <td>21</td>
                <td>2011/12/12</td>
                <td>$106,450</td>
                <td>8330</td>
                <td>c.vance@datatables.net</td>
              </tr>

              <tr>
                <td>Doris</td>
                <td>Wilder</td>
                <td>Sales Assistant</td>
                <td>Sidney</td>
                <td>23</td>
                <td>2010/09/20</td>
                <td>$85,600</td>
                <td>3023</td>
                <td>d.wilder@datatables.net</td>
              </tr>

              <tr>
                <td>Angelica</td>
                <td>Ramos</td>
                <td>Chief Executive Officer (CEO)</td>
                <td>London</td>
                <td>47</td>
                <td>2009/10/09</td>
                <td>$1,200,000</td>
                <td>5797</td>
                <td>a.ramos@datatables.net</td>
              </tr>

              <tr>
                <td>Gavin</td>
                <td>Joyce</td>
                <td>Developer</td>
                <td>Edinburgh</td>
                <td>42</td>
                <td>2010/12/22</td>
                <td>$92,575</td>
                <td>8822</td>
                <td>g.joyce@datatables.net</td>
              </tr>

              <tr>
                <td>Jennifer</td>
                <td>Chang</td>
                <td>Regional Director</td>
                <td>Singapore</td>
                <td>28</td>
                <td>2010/11/14</td>
                <td>$357,650</td>
                <td>9239</td>
                <td>j.chang@datatables.net</td>
              </tr>

              <tr>
                <td>Brenden</td>
                <td>Wagner</td>
                <td>Software Engineer</td>
                <td>San Francisco</td>
                <td>28</td>
                <td>2011/06/07</td>
                <td>$206,850</td>
                <td>1314</td>
                <td>b.wagner@datatables.net</td>
              </tr>

              <tr>
                <td>Fiona</td>
                <td>Green</td>
                <td>Chief Operating Officer (COO)</td>
                <td>San Francisco</td>
                <td>48</td>
                <td>2010/03/11</td>
                <td>$850,000</td>
                <td>2947</td>
                <td>f.green@datatables.net</td>
              </tr>

              <tr>
                <td>Shou</td>
                <td>Itou</td>
                <td>Regional Marketing</td>
                <td>Tokyo</td>
                <td>20</td>
                <td>2011/08/14</td>
                <td>$163,000</td>
                <td>8899</td>
                <td>s.itou@datatables.net</td>
              </tr>

              <tr>
                <td>Michelle</td>
                <td>House</td>
                <td>Integration Specialist</td>
                <td>Sidney</td>
                <td>37</td>
                <td>2011/06/02</td>
                <td>$95,400</td>
                <td>2769</td>
                <td>m.house@datatables.net</td>
              </tr>

              <tr>
                <td>Suki</td>
                <td>Burks</td>
                <td>Developer</td>
                <td>London</td>
                <td>53</td>
                <td>2009/10/22</td>
                <td>$114,500</td>
                <td>6832</td>
                <td>s.burks@datatables.net</td>
              </tr>

              <tr>
                <td>Prescott</td>
                <td>Bartlett</td>
                <td>Technical Author</td>
                <td>London</td>
                <td>27</td>
                <td>2011/05/07</td>
                <td>$145,000</td>
                <td>3606</td>
                <td>p.bartlett@datatables.net</td>
              </tr>

              <tr>
                <td>Gavin</td>
                <td>Cortez</td>
                <td>Team Leader</td>
                <td>San Francisco</td>
                <td>22</td>
                <td>2008/10/26</td>
                <td>$235,500</td>
                <td>2860</td>
                <td>g.cortez@datatables.net</td>
              </tr>

              <tr>
                <td>Martena</td>
                <td>Mccray</td>
                <td>Post-Sales support</td>
                <td>Edinburgh</td>
                <td>46</td>
                <td>2011/03/09</td>
                <td>$324,050</td>
                <td>8240</td>
                <td>m.mccray@datatables.net</td>
              </tr>

              <tr>
                <td>Unity</td>
                <td>Butler</td>
                <td>Marketing Designer</td>
                <td>San Francisco</td>
                <td>47</td>
                <td>2009/12/09</td>
                <td>$85,675</td>
                <td>5384</td>
                <td>u.butler@datatables.net</td>
              </tr>
              
              <tr>
                <td>Howard</td>
                <td>Hatfield</td>
                <td>Office Manager</td>
                <td>San Francisco</td>
                <td>51</td>
                <td>2008/12/16</td>
                <td>$164,500</td>
                <td>7031</td>
                <td>h.hatfield@datatables.net</td>
              </tr>

              <tr>
                <td>Hope</td>
                <td>Fuentes</td>
                <td>Secretary</td>
                <td>San Francisco</td>
                <td>41</td>
                <td>2010/02/12</td>
                <td>$109,850</td>
                <td>6318</td>
                <td>h.fuentes@datatables.net</td>
              </tr>

              <tr>
                <td>Vivian</td>
                <td>Harrell</td>
                <td>Financial Controller</td>
                <td>San Francisco</td>
                <td>62</td>
                <td>2009/02/14</td>
                <td>$452,500</td>
                <td>9422</td>
                <td>v.harrell@datatables.net</td>
              </tr>

              <tr>
                <td>Timothy</td>
                <td>Mooney</td>
                <td>Office Manager</td>
                <td>London</td>
                <td>37</td>
                <td>2008/12/11</td>
                <td>$136,200</td>
                <td>7580</td>
                <td>t.mooney@datatables.net</td>
              </tr>

              <tr>
                <td>Jackson</td>
                <td>Bradshaw</td>
                <td>Director</td>
                <td>New York</td>
                <td>65</td>
                <td>2008/09/26</td>
                <td>$645,750</td>
                <td>1042</td>
                <td>j.bradshaw@datatables.net</td>
              </tr>

              <tr>
                <td>Olivia</td>
                <td>Liang</td>
                <td>Support Engineer</td>
                <td>Singapore</td>
                <td>64</td>
                <td>2011/02/03</td>
                <td>$234,500</td>
                <td>2120</td>
                <td>o.liang@datatables.net</td>
              </tr>

              <tr>
                <td>Bruno</td>
                <td>Nash</td>
                <td>Software Engineer</td>
                <td>London</td>
                <td>38</td>
                <td>2011/05/03</td>
                <td>$163,500</td>
                <td>6222</td>
                <td>b.nash@datatables.net</td>
              </tr>

              <tr>
                <td>Sakura</td>
                <td>Yamamoto</td>
                <td>Support Engineer</td>
                <td>Tokyo</td>
                <td>37</td>
                <td>2009/08/19</td>
                <td>$139,575</td>
                <td>9383</td>
                <td>s.yamamoto@datatables.net</td>
              </tr>

              <tr>
                <td>Thor</td>
                <td>Walton</td>
                <td>Developer</td>
                <td>New York</td>
                <td>61</td>
                <td>2013/08/11</td>
                <td>$98,540</td>
                <td>8327</td>
                <td>t.walton@datatables.net</td>
              </tr>

              <tr>
                <td>Finn</td>
                <td>Camacho</td>
                <td>Support Engineer</td>
                <td>San Francisco</td>
                <td>47</td>
                <td>2009/07/07</td>
                <td>$87,500</td>
                <td>2927</td>
                <td>f.camacho@datatables.net</td>
              </tr>

              <tr>
                <td>Serge</td>
                <td>Baldwin</td>
                <td>Data Coordinator</td>
                <td>Singapore</td>
                <td>64</td>
                <td>2012/04/09</td>
                <td>$138,575</td>
                <td>8352</td>
                <td>s.baldwin@datatables.net</td>
              </tr>

              <tr>
                <td>Zenaida</td>
                <td>Frank</td>
                <td>Software Engineer</td>
                <td>New York</td>
                <td>63</td>
                <td>2010/01/04</td>
                <td>$125,250</td>
                <td>7439</td>
                <td>z.frank@datatables.net</td>
              </tr>

              <tr>
                <td>Zorita</td>
                <td>Serrano</td>
                <td>Software Engineer</td>
                <td>San Francisco</td>
                <td>56</td>
                <td>2012/06/01</td>
                <td>$115,000</td>
                <td>4389</td>
                <td>z.serrano@datatables.net</td>
              </tr>
              
              <tr>
                <td>Jennifer</td>
                <td>Acosta</td>
                <td>Junior Javascript Developer</td>
                <td>Edinburgh</td>
                <td>43</td>
                <td>2013/02/01</td>
                <td>$75,650</td>
                <td>3431</td>
                <td>j.acosta@datatables.net</td>
              </tr>

              <tr>
                <td>Cara</td>
                <td>Stevens</td>
                <td>Sales Assistant</td>
                <td>New York</td>
                <td>46</td>
                <td>2011/12/06</td>
                <td>$145,600</td>
                <td>3990</td>
                <td>c.stevens@datatables.net</td>
              </tr>

              <tr>
                <td>Hermione</td>
                <td>Butler</td>
                <td>Regional Director</td>
                <td>London</td>
                <td>47</td>
                <td>2011/03/21</td>
                <td>$356,250</td>
                <td>1016</td>
                <td>h.butler@datatables.net</td>
              </tr>

              <tr>
                <td>Lael</td>
                <td>Greer</td>
                <td>Systems Administrator</td>
                <td>London</td>
                <td>21</td>
                <td>2009/02/27</td>
                <td>$103,500</td>
                <td>6733</td>
                <td>l.greer@datatables.net</td>
              </tr>

              <tr>
                <td>Jonas</td>
                <td>Alexander</td>
                <td>Developer</td>
                <td>San Francisco</td>
                <td>30</td>
                <td>2010/07/14</td>
                <td>$86,500</td>
                <td>8196</td>
                <td>j.alexander@datatables.net</td>
              </tr>

              <tr>
                <td>Shad</td>
                <td>Decker</td>
                <td>Regional Director</td>
                <td>Edinburgh</td>
                <td>51</td>
                <td>2008/11/13</td>
                <td>$183,000</td>
                <td>6373</td>
                <td>s.decker@datatables.net</td>
              </tr>

              <tr>
                <td>Michael</td>
                <td>Bruce</td>
                <td>Javascript Developer</td>
                <td>Singapore</td>
                <td>29</td>
                <td>2011/06/27</td>
                <td>$183,000</td>
                <td>5384</td>
                <td>m.bruce@datatables.net</td>
              </tr>

              <tr>
                <td>Donna</td>
                <td>Snider</td>
                <td>Customer Support</td>
                <td>New York</td>
                <td>27</td>
                <td>2011/01/25</td>
                <td>$112,000</td>
                <td>4226</td>
                <td>d.snider@datatables.net</td>
              </tr>
            </tbody>
          </table>
        </div>
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
      email: "",
      password: "",
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