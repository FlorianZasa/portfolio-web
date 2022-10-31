<template>
  <div class="window">
    <div id="nav">
      <router-link class="router-link" to="/">Home</router-link>
      <router-link class="router-link" to="/about">Über mich</router-link>
      <router-link class="router-link" to="/contact">Kontakt</router-link>
    </div>
    <router-view class="content"/>
  </div>
  <footer>
    <p>© 2022 Florian Zasada</p>
  </footer>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #2c3e50;
}

.content {
  padding: 3vw;
  width: 78vw
}

.window {
  display: inline-flex;
  height: 100%
}

#nav {
  padding-top: 5vw;
  width: 22vw;
  background-color: #25313e;
  border-radius: 0 0 20px 0;
  display:flex;
  flex-direction: column;
}

footer {
  padding: 3vw;
  display: flex;
  justify-content: center;
  background: #2c3948;
}

#nav .router-link {
  color: var(--secondary-fg);
  font-size: 2vw;
  width: 100%;
  border-bottom: 2px solid #4c5053;
  text-align: center;
  margin: 10px;
  
  background: linear-gradient(to left, #25313e, rgb(107, 119, 59) 99%) right;
  background-size: 200% 100%;
  position: relative;
}

#nav .router-link:hover {
  transition: all 1s ease-in-out;
  background-position: left;
  color: var(--fg-text);
  width: 120%;
}

</style>
