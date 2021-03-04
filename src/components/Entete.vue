<template>
  <header>
    <h1 @click="openHome()">Julie Gobin</h1>
    <div class="filet"></div>
  </header>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Entete',
  components: {
    
  }, 
  methods:{
    openHome() {
      this.$emit('affichageHome')
    },
  }
}
</script>

<style lang="scss">

@import "../sass/main.scss";

header {
    // position: relative;
    // left: 0px;
    z-index: 5;
    // transition: transform 1.5s cubic-bezier(.25, .1, .25, 1);
    // transform: translate(830px, 0px);
    animation-name: anim-header;
    animation-duration: 1.5s;
    animation-fill-mode: forwards;
    @include mobile{
      width: 100%;
      // left: 0;
      // position: inherit;
      animation: none;
    }
}
@keyframes anim-header{
    from {
        transform: translate(-830px, 0px);
    }
    to {
        transform: translate(0px, 0px);
    }
}

h1 {
    font-family: $serif;
    font-size: 5rem;
    font-weight: 400;
    text-align: left;
    max-width: 980px;
    margin: auto;
    color: $firstColor; 
    @include mobile{
      font-size: 2rem;
    }  
}

.filet{
    height: 3px;
    width: 46%;
    background-color: $firstColor;
    @include mobile{
      width: 58%;
    }
}



</style>
