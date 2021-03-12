<template>
  <section class="contact">
    <h3>Pour me joindre :</h3>  
    <div class="liste">
        <!-- <p>Téléphone : 06 07 82 42 12 <br/>
        <a href="mailto:julie.gobin1106@gmail.com">Email : julie.gobin1106@gmail.com</a><br/> -->
        <a href="https://www.linkedin.com/in/julie-gobin-a6b1ab1a3/">LinkedIn</a>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Contact',
  components: {
    
  }
}
</script>

<style lang="scss">

@import "../sass/main.scss";

.contact {
    margin-top: 5%;
    text-align: center;
    h3{
    font-size: 1.5rem; 
    }
  .liste{
    margin-top: 5%;
    p{ 
    font-family: $serif;
    font-weight: 200;
    font-size: 1.2rem;
    line-height: 3rem;
    color: $firstColor;
    }
    a {
        text-decoration: none;
        color: $firstColor;
        &:hover{
            color: $quatreColor;
            text-decoration: underline;
            font-weight: 500;
        }
    }
  }
}








</style>
