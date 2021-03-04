<template>
  <section>
    <div id="illustr">
    <img src="../assets/illustr.png"/>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Prez',
  components: {
    
  }
}
</script>

<style lang="scss">

@import "../sass/main.scss";

  #illustr {
    // position: absolute;
    // top: -8px;
    width: 40%;
    right: 25%;
    animation-name: anim-illust;
    animation-duration: 1.5s;
    animation-fill-mode: forwards;
  img{
    width: 80%;
  }
  @include mobile{
    display: none;
  }
  }

    p {
        text-align: center;
        font-family: $serif;

    }

    .signe {
        color: $secondColor;
        font-size: 15rem;
        font-weight: 900;
        opacity: 0.5;
    }

    @keyframes anim-illust{
    from {
        transform: translate(2830px, 0px);
    }
    to {
        transform: translate(50px, 0px);
    }
}









</style>
