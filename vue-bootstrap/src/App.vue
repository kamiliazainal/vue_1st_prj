<template>
  <div id="app">
    <div class="container">
      <!-- Header -->
        <b-jumbotron class="jumbotron" id="gambar1">
        </b-jumbotron>
      <!-- End Header -->
    <!-- Navbar -->
      <b-navbar toggleable="lg" type="light" class="navbar">
        <b-navbar-brand href="#">NavBar</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item href="#">Link</b-nav-item>
            <b-nav-item href="#" disabled>Disabled</b-nav-item>
          </b-navbar-nav>

          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-nav-form>
              <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
              <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
            </b-nav-form>

            <b-nav-item-dropdown text="Lang" right>
              <b-dropdown-item href="#">EN</b-dropdown-item>
              <b-dropdown-item href="#">ES</b-dropdown-item>
              <b-dropdown-item href="#">RU</b-dropdown-item>
              <b-dropdown-item href="#">FA</b-dropdown-item>
            </b-nav-item-dropdown>

            <b-nav-item-dropdown right>
              <!-- Using 'button-content' slot -->
              <template v-slot:button-content>
                <em>User</em>
              </template>
              <b-dropdown-item href="#">Profile</b-dropdown-item>
              <b-dropdown-item href="#">Sign Out</b-dropdown-item>
            </b-nav-item-dropdown>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    <!-- End navbar -->
    <!-- Body -->
    <div class="container"> 
      <b-container class="bv-example-row">
        <b-row>
          <b-col cols="3">
           
              <b-img src="https://techaccess.org/wp-content/uploads/2019/03/network-for-edwork-web-banner-vertical.png" fluid alt="Responsive image"></b-img>
         
          </b-col>
          <b-col cols="6">
           
              <b-img src="https://images.unsplash.com/photo-1489844097929-c8d5b91c456e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&w=1000&q=80" fluid alt="Responsive image"></b-img>
           
          </b-col>
          <b-col cols="3">
           
              <b-img src="https://techaccess.org/wp-content/uploads/2019/03/network-for-edwork-web-banner-vertical.png" fluid alt="Responsive image"></b-img>
           
          </b-col>
        </b-row>
      </b-container>
      </div>
    <!-- End body -->

    <!-- kalau taknak guna style bootstrap-vue, pakai je cara sama
      <div class="container">
      <div class="row">
        <div class="col">1 of 3</div>
        <div class="col">2 of 3</div>
        <div class="col">3 of 3</div>
      </div>
    </div> -->
  </div>
  </div>
</template>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.jumbotron .jumbotron-fluid{
  height:100%;
}

#gambar1 {
  background-image: url(https://www.williamstownfarmersmarket.org/wp-content/uploads/2013/01/header-man2.jpg);
}

.navbar {
  background-color:rgb(213, 231, 236);
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
