<template>
<div class="slide">
    <div class="carre" @click="affMget()"></div>
    <div class="carre" @click="affIrm()"></div>
    <div class="carre" @click="affMoulin()"></div>
    <div class="carre" @click="affArc()"></div>
    <div class="carre" @click="affSarre()"></div>
    <div class="carre" @click="affOhara()"></div>
    <div class="carre" @click="affLepape()"></div>
    <div class="carre" @click="affCanal()"></div>
    <div class="carre" @click="affSDMO()"></div>
    <div class="carre" @click="affPozzo()"></div>
    <div class="carre" @click="affLogicmax()"></div>
</div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Next',
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


.slide{
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    width: 40%;
    margin-left: 3%;
}

.carre {

    width:15px;
    height: 15px;
    background-color: $secondColor;
    transition: transform 400ms;
    &:hover {
        transform: scale(1.15);
        background-color: $quatreColor;
    }

    p{
        text-align: center;
        color: #fff;
        font-weight: 900;
        font-size: 2rem;
    }
}




</style>
