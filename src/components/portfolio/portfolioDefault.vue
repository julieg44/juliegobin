<template>
<div id="portfolioIntro">
    <h3>Mon parcours en images…</h3>
    <p>15 ans d'infographie <br/>et une formation de développeur <br/></p>
</div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'portfolioDefault',
  components: {
    
  }
}
</script>

<style lang="scss">

@import "../../sass/main.scss";

#portfolioIntro{
    margin-top: 20%;
    text-align: center;
    p{
        font-family: $serif;
        font-size: 1rem;
    }
}









</style>
