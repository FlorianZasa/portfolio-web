<template>
    <div class="home">
      <div class="header-frame">
          <h1>Erfahre mehr</h1>
          <h2>über mich</h2>
      </div>
      <div class="spacer"></div>
      
      <div class="subtitle-frame">
        <h4>2019 - März 2023</h4>
        <p>Studium - Bachelor of Engineering - Telekommunikationsinformatik</p>
      </div>
      <div class="spacer"></div>
      <div class="subtitle-frame">
        <h4>2023 - heute</h4>
        <p>Studium - Master of Science - Cyber Security</p>
      </div>
      <div class="spacer"></div>
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
    align-items: center;
    width: 100%; 
  }
  
  .spacer{
    padding-bottom: 4vw;
  }
  
  .title-frame {
    align-items: center;
    width: 60%; 
  }
  
  .title-frame img {
    width: 100%;
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
  