<template>
  <div id="app">
    <div>
  <b-navbar toggleable="lg" type="light" style="border: #2a2e43;" variant="white">
    <b-navbar-brand >
      <img
                  style="height: 40px"
                  src="./assets/Screenshot_20220321-202438_Chrome.jpg"
                />
    </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
      <b-nav-item to="/" >About</b-nav-item>
      <b-nav-item onClick="location.href='https://educateachild.org/explore/barriers-to-education/resources'" >Resources</b-nav-item>
        <b-nav-item onClick="location.href='https://www.naijanews.com/'" > Blog</b-nav-item>
        
      </b-navbar-nav>
      <b-navbar-nav class="ml-auto">
        <div>
          <b-row>
            <b-col lg="4">
     <router-link to="/login" class="line" > <button size="sm" class="btn" style="box-shadow:none;color:#09BD80"  > Login</button></router-link>
      </b-col>
      <b-col >
      <router-link to="/signup" class="line" > <button size="sm" class="btn" style="box-shadow:none;color:#09BD80">Sign Up</button> </router-link>
      </b-col>
          </b-row>
      </div>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
  <hr>
</div>

    <router-view/>
  </div>
</template>
<script>

export default {
  
};
</script>

<style lang="scss">
#app {
  font-family: 'Nunito Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #29292B;
}

#nav {
  padding: 0px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

.btn {
  background-color: white; 
  color: #09BD80; 
  border: none;
}

.btn:hover {
  background-color: #09BD801A;
  color: white;
}

.line{
  text-decoration: none;
  color: inherit;
}
</style>
