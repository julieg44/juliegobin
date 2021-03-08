<template>
<div class="tableau">
    <div class="vignette" @click="affMget()"><img class="contain color" src="../../assets/MGET.png" alt="MGET"/><img class="contain NB" src="../../assets/MGET-NB.png" alt="MGET - noir et blanc"/></div>
    <div class="vignette" @click="affIrm()"><img class="contain color" src="../../assets/IRM-mini.png" alt="IRM"/><img class="contain NB" src="../../assets/IRM-mini-NB.png" alt="IRM - noir et blanc"/></div>
    <div class="vignette" @click="affMoulin()"><img class="contain color" src="../../assets/moulin.png" alt="Moulin"/><img class="contain NB" src="../../assets/moulin-NB.png" alt="Moulin - noir et blanc"/></div>
    <div class="vignette" @click="affArc()"><img class="contain color" src="../../assets/arc-mini.jpg" alt="Arc"/><img class="contain NB" src="../../assets/arc-mini-NB.jpg" alt="Arc - noir et blanc"/></div>
    <div class="vignette" @click="affSarre()"><img class="contain color" src="../../assets/sarre-mini.gif" alt="sarre"/><img class="contain NB" src="../../assets/sarre-mini-NB.gif" alt="sarre - noir et blanc"/></div>
    <div class="vignette" @click="affOhara()"><img class="contain color" src="../../assets/ohara-mini.jpg" alt="ohara"/><img class="contain NB" src="../../assets/ohara-mini-NB.jpg" alt="ohara - noir et blanc"/></div>
    <div class="vignette" @click="affLepape()"><img class="contain color" src="../../assets/catalogue/MES.png" alt="catalogue"/><img class="contain NB" src="../../assets/catalogue/MES-NB.png" alt="catalogue - noir et blanc"/></div>
    <div class="vignette" @click="affCanal()"><img class="contain color" src="../../assets/canal/GIF_CANAL.gif" alt="canal"/><img class="contain NB" src="../../assets/canal/GIF_CANAL-NB.gif" alt="canal - noir et blanc"/></div>
    <div class="vignette" @click="affSDMO()"><img class="contain color" src="../../assets/SDMO/SDMO-landing.jpg" alt="SDMO"/><img class="contain NB" src="../../assets/SDMO/SDMO-landing-NB.jpg" alt="SDMO - noir et blanc"/></div>
    <div class="vignette" @click="affPozzo()"><img class="contain color" src="../../assets/pozzo/pozzo.gif" alt="pozzo"/><img class="contain NB" src="../../assets/pozzo/pozzo-NB.gif" alt="pozzo - noir et blanc"/></div>
    <div class="vignette" @click="affLogicmax()"><img class="contain color" src="../../assets/logicmax/logicmax.gif" alt="logicmax"/><img class="contain NB" src="../../assets/logicmax/logicmax-NB.gif" alt="logicmax - noir et blanc"/></div>
</div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'graphismeIntro',
  methods: {
    affMget() {
      this.$emit('One')
    },
    affIrm() {
      this.$emit('Two')
    },
    affMoulin() {
      this.$emit('Three')
    },
    affArc() {
      this.$emit('Four')
    },
    affSarre() {
      this.$emit('Five')
    },
    affOhara() {
      this.$emit('Six')
    },
    affLepape() {
      this.$emit('Seven')
    },
    affCanal() {
      this.$emit('Eight')
    },
    affSDMO() {
      this.$emit('Nine')
    },
    affPozzo() {
      this.$emit('Ten')
    },
    affLogicmax() {
      this.$emit('Eleven')
    }
  }
}
</script>

<style lang="scss">

@import "../../sass/main.scss";


.tableau{
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    flex-wrap: wrap;
}

.vignette {
    border: 1px solid black;
    width:30%;
    margin-bottom: 3%;
    margin-right: 3%;
    transition: transform 400ms;
    text-align: center;
    background-color: #fff;
    padding: 2%;
    cursor: pointer;
    @include mobile {
      width: 47%;
    }
    img{
        transition: transform 400ms;
        width: 150px;
        height: 150px;
    }
    .contain{
        object-fit: contain;
    }
    .color{
        display: none;
    }
    &:hover {
        transform: scale(1.15);
        padding: 3%;
        img{
        transform: scale(1.15);
        }
        .contain{
        object-fit: contain;
    }
        .NB{
            display: none;
        }
        .color{
            display: block;
        }
    }

    p{
        text-align: center;
        color: #fff;
        font-weight: 900;
        font-size: 2rem;
    }
}




</style>
