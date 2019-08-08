<template>
  <div id="app">
    <div class="container fluid">
      <div class="row">
        <div class="column left">
          <div id="nav">
            <h1>Bailee Mulholland</h1>
            <router-link to="/resume">Resume</router-link>
            <br />
            <router-link to="/about">About</router-link>
          </div>
        </div>
        <div class="colomn right">
          <router-view />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {}
};
</script>


<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #9e9393;
}
#nav {
  font-size: 20px;
  display: block;
  align-content: left;
}

#nav a {
  color: #e6d0d0;
  padding: 20px;
}

#nav a.router-link-exact-active {
  color: #9e9393;
  font-weight: bold;
}
.colomn {
  float: left;
  padding: 4em;
}
.left {
  width: 20%;
  align-content: left;
  text-align: left;
  padding-top: 10em;
  display: block;
  padding-right: 0em;
  margin-right: 0em;
}

.right {
  width: 80%;
  align-content: left;
  /* display: inline; */
  padding-top: 4em;
  text-align: left;
}

.row:after {
  content: "";
  display: table;
  clear: both;
}

body {
  background-color: whitesmoke;
}

#third_one {
  margin-top: 10%;
  max-width: 25%;
}
</style>
