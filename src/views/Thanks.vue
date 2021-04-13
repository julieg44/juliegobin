<template>
  <div class="thanks">
    <h1 class="thanks-titre">Merci de m'avoir contactée ;)</h1>
    <p class="thanks-text">Je reprends contact très vite, <br>à bientôt !</p>
    <div id="back"><a href='/'>Back</a></div>
  </div>
</template>


<script>
export default {
  name: 'Thanks'
  }
</script>

<style lang="scss">

@import "../sass/main.scss";

.thanks {
  text-align: center;
  margin: auto;
  margin-top: 30%;
  .thanks-titre{ 
  font-size: 2rem;
  color: $quatreColor;
  text-align: center;
  }
  .thanks-text{ 
  font-size: 1.3rem;
  text-align: center;
  }
  #back{
    margin-bottom: 15%;
    font-size: 1rem;
    color: $quatreColor;
  }
}
</style>
