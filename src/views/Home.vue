<template>
  <div class="home">
    <div class="header-frame">
      <div class="title-frame">
        <h1>Willkommen!</h1>
        <h1>ich bin <span><img src="../assets/fz.gif"/></span></h1>
      </div>
      <div class="image-frame">
        <img src="../assets/flo.png" />
        <div class="middle">
          <div class="text">"Hi! Schön, dass du hier bist! Erfahre hier mehr von mir!"</div>
        </div>
      </div>
    </div>
    <div class="spacer"></div>
    
    <div class="subtitle-frame">
      <h4><span class="fancy">Software Entwickler</span> in den Bereichen Python, Java, sowie Frontendentwicklung mit HTML, CSS, JS und bekannten Frameworks wie Vue.js oder React.js.</h4>
    </div>
    <div class="spacer"></div>

    <div class="links-frame">
      <button type="button">Erfahre mehr über mich</button>
    </div>
    <div class="spacer"></div>
    <div class="subtitle-frame">
      <h4>Brauchst du eine Webseite, eine Automatisierungs- oder Managementsoftware o.ä.?</h4>
      <p>Kontaktiere mich direkt <a href='#'>hier</a>!</p>
      <p>Falls dich meine bisherigen Projekte interessieren, dann schau doch mal <a href="#">hier</a> vorbei.</p>
    <div class="spacer"></div>
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
  width: 100%;
}

button {
  font-size: 100%;
}
.header-frame {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  margin-top: 10%;
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
  position: relative;
}
.image-frame img {
  width: 50%;
  height: auto;
  border:4px solid var(--secondary-fg);
  border-radius: 20px;
  opacity: 1;
  transition: .5s ease;
  backface-visibility: hidden;
}

.image-frame:hover img {
  opacity: 0.3;
  width: 70%;
}

.image-frame:hover .middle {
  opacity: 1;
}

.middle {
  transition: .5s ease;
  opacity: 0;
  font-size: 2vw;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%)
}



@media only screen and (max-width: 600px) {
  .header-frame {
    flex-direction: column;
  }

  .image-frame {
    justify-content: center;
  }

  .image-frame img {
    width: 100%;
    height: auto;
  }

  .image-frame:hover img {
    opacity: 0.3;
  }
  .image-frame:hover .middle {
    font-size: 14px;
    width: 100%;
  }

  .title-frame {
    align-items: center;
    width: 80%; 
  }
}
</style>
