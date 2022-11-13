<template>
  <div class="window">
    <nav class="nav">
      <router-link class="nav-link" to="/">Home</router-link>
      <div id="myLinks">
        <router-link class="nav-link" to="/about">Über mich</router-link>
        <router-link class="nav-link" to="/contact">Kontakt</router-link>
      </div>
      <a href="javascript:void(0);" class="icon nav-link" @click="myFunction()">
        <i class="fa-solid fa-bars"></i>

        <i class="fa fa-bars"></i>
      </a>
    </nav>
    <div class="container">
      <router-view class="content"/>
    </div>
  </div>
  <footer>
    <p>© 2022 Florian Zasada</p>
  </footer>
</template>

<script>
 
 export default {
  name: "App",
  methods: {
    myFunction() {
      var x = document.getElementById("myLinks");
      if (x.style.display === "block") {
        x.style.display = "none";
      } else {
        x.style.display = "block";
      }
    }
  }
 }
  </script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: var(--bg);
}

.nav {
  display: flex;
  flex-direction: row;
  background: var(--dark-bg);
}

.nav a {
  color: white;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
  display: block;
}

#myLinks{
  display: flex;
  flex-direction: row;
}


footer{
  background: var(--dark-bg);
  padding: 20px;
}



@media only screen and (max-width: 600px) {

  .window {
    display: flex;
    flex-direction: column;
    height: 100%;
    max-width: 480px;
    color: white;
    border-radius: 10px;
  }
  .nav {
    display:flex;
    flex-direction: column;
    padding-top: 0px;
    width: 100%;
    overflow: hidden;
    position: relative;
  }

  .nav a.icon {
  background: black;
  display: block;
  position: absolute;
  right: 0;
  top: 0;
}


.nav #myLinks {
  display: none;
}

.nav a {
  color: white;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
  display: block;
}

.nav a.icon {
  background: black;
  display: block;
  position: absolute;
  right: 0;

}

}
</style>
