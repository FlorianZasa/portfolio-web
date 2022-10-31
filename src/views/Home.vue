<template>
  <div class="home">
    <div class="header-frame">
      <div class="title-frame">
        <h1>Willkommen!</h1>
        <h1>ich bin <span><img src="../assets/fz.gif"/></span></h1>
      </div>
      <div class="image-frame">
        <img src="../assets/flo.png" />
      </div>
    </div>
    <div class="spacer"></div>
    
    <div class="subtitle-frame">
      <h4><span class="fancy">Software Entwickler</span> in den Bereichen Python, Java, sowie Frontendentwicklung mit HTML, CSS, JS und bekannten Frameworks wie Vue.js oder React.js.</h4>
    </div>
    <div class="spacer"></div>

    <div class="links-frame">
      <button type="button" class="btn btn-primary">Erfahre mehr über mich</button>
    </div>
    <div class="spacer"></div>

    <div class="purchase-frame">
      <h5>Brauchst du eine Webseite, eine Automatisierungs- oder Managementsoftware o.ä.?</h5>
      <p>Kontaktiere mich direkt <a href='#'>hier</a>!</p>
      <p>Falls dich meine bisherigen Projekte interessieren, dann schau doch mal <a href="#">hier</a> vorbei.</p>
    </div>
    
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@300&display=swap');

.home {
  align-items: center;
  text-align: center;
}

.header-frame {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.spacer{
  padding-bottom: 4vw;
}

.title-frame {
  align-items: center;
  width: 60%; 
}

.title-frame img {
  width: 90%;
}

.fancy {
  font-weight: bold;
  font-family: 'Roboto Mono', monospace;
  color: var(--secondary-fg);
  font-weight: bold;
}

.image-frame {
  width: 40%;
  padding: 0px;
  margin: 0px;
}
.image-frame img {
  width: 50%;
  height: auto;
  border:4px solid var(--secondary-fg);
  border-radius: 20px;
}
</style>
