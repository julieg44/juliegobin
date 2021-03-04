<template>
<div class="slide">
    <div class="carre" @click="affGroupomania()"></div>
</div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'NextDev',
  methods: {
    affGroupomania() {
      this.$emit('One')
    },
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
