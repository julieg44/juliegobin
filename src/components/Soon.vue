<template>
  <section>
    <div id="soon">
        <div class="load">
            <div class="load__dot load__dot--1"></div>
            <div class="load__dot load__dot--2"></div>
            <div class="load__dot load__dot--3"></div>
        </div>
    <p>La version mobile arrive très prochainement !!<br/>
    pourquoi ne pas jeter un oeil à mon site sur un ordinateur en attendant ? ;)</p>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Soon',
  components: {
    
  }
}
</script>

<style lang="scss">

@import "../sass/main.scss";

$size-dot: 2.5vh;
$size-dot-mobile: 1.5vh;
$anim-dur: 1000ms;
$num-dot : 3;
$anim-delay: $anim-dur / $num-dot;

#soon{
    width: 70%;
    margin-top: 20%;
    p{
        width: 71%;
        text-align: center;
        margin: auto;
        margin-top: 5%;
    }
}

.load {
    width: $size-dot-mobile*5;
    height: $size-dot-mobile;
    display: flex;
    justify-content: space-evenly;
    margin-top: 2%;
    margin: auto;
    @include tablette_ecran{
        width: $size-dot*5;
        height: $size-dot;
        margin-top: 0%;
    }

    &__dot {
        background-color: $secondColor;
        height: 100%;
        width: $size-dot-mobile;
        border-radius: 15px;
        animation: dot $anim-dur backwards infinite;
        animation-direction: alternate;
        @include tablette_ecran{
            width: $size-dot;
        }

        @for $i from 1 through $num-dot {
            &--#{$i} {
                animation-delay: $anim-delay * $i;
            }
        }
    }
}

@keyframes dot {
    0% {
        transform: scaleY(0.5) scaleX(0.5);
        transform-origin: center;
    }

    100% {
        transform: scaleY(1) scaleX(1);
        transform-origin: center;
    }
}








</style>
