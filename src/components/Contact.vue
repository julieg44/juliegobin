<template>
  <section class="contact">
    <h3>Pour me joindre :</h3>  
    <div class="liste">
        <!-- <p>Téléphone : 06 07 82 42 12 <br/>
        <a href="mailto:julie.gobin1106@gmail.com">Email : julie.gobin1106@gmail.com</a><br/> -->
        <img src="../assets/linkedIn.png" alt="linkedIn" id="linkedIn"/><a href="https://www.linkedin.com/in/julie-gobin-a6b1ab1a3/">LinkedIn</a>
    </div>
      <form id="formulaire" name="contact" method="POST" data-netlify="true">
        <input type="hidden" name="form-name" value="contact">

        <p class="flex-form">
          <label>Votre nom: <input type="text" name="name" /></label>
        </p>
        <p class="flex-form">
          <label>Votre Email: <input type="email" name="email" /></label>
        </p>
        <p class="flex-form">
          <label>Message: <textarea name="message"></textarea></label>
        </p>
        <p>
          <button id="envoyer" type="submit">Envoyer</button>
        </p>
      </form>
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
    h3{
    font-size: 1.5rem;
    text-align: center; 
    }
    #linkedIn{
      width: 4%;
      margin-right: 1%;
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
  #formulaire{
    margin-top: 10%;
    text-align: center;
    .flex-form{
      display: flex;
    }
    input, textarea{
      width: 100%;
      height: 33px;
      border: none;
      background-color: $grey;
      color: #000;
    }
    textarea{
      height: 100px;
    }
    label{
      color: $thirdColor;
      font-weight: 700;
      width: 100%;
      text-align: left;
    }
    #envoyer{
      width: 35%;
      font-weight: 700;
      background-color: $thirdColor;
      color: $blanc;
      border: none;
      height: 40px;
      margin-top: 3%;
    }
  }
}








</style>
