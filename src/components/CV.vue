<template>
    <div id="cv">


        <!-- corps-->
        <section class="contenuCv">
            <header id="headerCv">
                <!--image ne doit s'afficher qu'en responsive-->
                <div id="identite_petit">
                    <img src="../assets/julieCV.jpg" alt="photo-d'identité"/>
                </div>
                <div id="identite">
                    <h1 class="nomCv"><span id="julie">Julie</span> Gobin</h1>
                    <h2>Développeur <span class="esperluette">&</span> graphiste</h2>
                    <div id="filet"></div>
                </div>
                <div id="layus">
                  <p>Comme je ne me suis pas trompée en débutant ma vie professionnelle par le graphisme, j'ai décidé de la poursuivre par du développement Web en entreprennant une formation dans ce domaine, sûre d'y trouver mon épanouissement. Imaginer des projets et leur donner vie, quoi de mieux en somme ?</p>
                </div>
            </header>

            <!--bloc expériences-->
            <article class="bloc_section">
                <div class="titre">
                    <i class="fas fa-suitcase"></i>
                    <h2 class="titreArticle">Expériences professionelles</h2>
                </div>
                <div class="ligne">
                    <div class="dates">
                        <i class="far fa-dot-circle"></i>
                        <p>Septembre 2018-Avril 2019<br />
                            Nantes</p>
                    </div>
                    <div class="contenu">
                        <h5>Diverses agences - interim</h5>
                        <p>Infographiste</p>
                        <p>- Mise en page de tracts publicitaires pour la grande distribution</p>
                        <p>- Mise en page de supports de communication dans le domaine de la promotion immobilière</p>
                    </div>
                </div>

                <div class="ligne">
                    <div class="dates">
                        <i class="fas fa-circle"></i>
                        <p>2015-2018<br />
                            Nantes</p>
                    </div>
                    <div class="contenu">
                        <h5>Agence LOOM</h5>
                        <p>Infographiste Web</p>
                        <p>- Création et déclinaison de pages pour sites et applications</p>
                        <p>- Création de bannières et gif animés</p>
                        <p>- Création et intégration d'emailings</p>
                    </div>
                </div>

                <div class="ligne">
                    <div class="dates">
                        <i class="fas fa-circle"></i>
                        <p>2008-2015<br />
                            Nantes</p>
                    </div>
                    <div class="contenu">
                        <h5>Agence LOOM</h5>
                        <p>Infographiste Print</p>
                        <p>- Maquettage de divers supports print (catalogues, affiches, mailings, flyers,
                            signalétiques…)</p>
                        <p>- Gestion de l'envoi en fabrication des supports</p>
                    </div>
                </div>

                <div class="ligne">
                    <div class="dates">
                        <i class="fas fa-circle"></i>
                        <p>2004-2008<br />
                            Couéron</p>
                    </div>
                    <div class="contenu">
                        <h5>Altavia Victor Communication</h5>
                        <p>Maquettiste éxé</p>
                        <p>- Maquettage de tracts publicitaires pour le compte de Système U</p>
                    </div>
                </div>
            </article>

            <!--bloc Formation-->
            <article class="bloc_section">
                <div class="titre">
                    <i class="fas fa-graduation-cap"></i>
                    <h2 class="titreArticle">Formations</h2>
                </div>
                <!--ligne 1-->
                <div class="ligne">

                    <div  class="dates">
                        <i class="far fa-dot-circle"></i>
                        <p>Janv 2020<br />
                            Nantes</p>
                    </div>
                    <div class="contenu">
                        <h5>Openclassrooms</h5>
                        <p>Diplôme de développeur web</p>
                    </div>
                </div>
                <!--ligne 2-->
                <div class="ligne">
                    <div class="dates">
                        <i class="fas fa-circle"></i>
                        <p>2001-2004<br />
                            Nantes</p>
                    </div>
                    <div class="contenu">
                        <h5>École Sépia arts graphiques</h5>
                        <p>Diplôme d'arts graphiques</p>
                    </div>
                </div>
                <!--ligne 3-->
                <div class="ligne">
                    <div class="dates">
                        <i class="fas fa-circle"></i>
                        <p>2000<br />
                            Nantes</p>
                    </div>
                    <div class="contenu">
                        <h5>Lycée Gabriel Guist'hau</h5>
                        <p>Baccalaureat L option arts plastiques </p>
                    </div>
                </div>
            </article>

            

            <!--recommandation-->
            <article class="bloc_section recommandation">
                <div class="titre">
                    <i class="fas fa-handshake"></i>
                    <h2 class="titreArticle">Recommandations</h2>
                </div>

                <div class="ligne_collegue">
                    <div class="collegue">
                        <h5>Julien Lepriol - Colin</h5>
                        <p>agence I5</p>
                        <p><a href="mailto:julien@i5.agency">julien@i5.agency</a></p>
                    </div>

                    <!-- <div class="collegue">
                        <h2>Damien Huteau</h2>
                        <p>agence I5</p>
                        <p><a href="mailto:xoxoxo@gmail.com#">email à compléter</a></p>
                    </div> -->
                </div>
            </article>
        </section>
        <!-- partie gauche -->
        <aside>
            <div id="photoIdentite">
                <p>
                    <img src="../assets/julieCV.jpg" alt="photo_identite" />
                </p>
            </div>
            <div id="contact">
                <h1>Contact</h1>
                <div class="contenuContact">
                  <p><a href="mailto:xoxoxo@gmail.com">julie.gobin1106@gmail.com</a></p>
                  <p>06 07 82 42 12</p>
                  <p>Permis B, vehiculée</p>   
                  <p><a href="https://juliegobin.netlify.app/">Mon site</a></p>
                  <p><a href="https://www.linkedin.com/in/julie-gobin-a6b1ab1a3/">LinkedIn</a></p>
                </div>
            </div>
            <div>
                <h1 class="titreLogiciels">Logiciels & languages maitrisés</h1>
                <ul>
                  <li class="logiciels"><div><p>InDesign</p></div><div>.............</div><div><p>confirmé</p></div></li>
                  <li class="logiciels"><div><p>Illustrator</p></div><div>...........</div><div><p>confirmé</p></div></li>
                  <li class="logiciels"><div><p>Photoshop</p></div><div>.........</div><div><p>confirmé</p></div></li>
                  <li class="logiciels"><div><p>HTML</p></div><div>........</div><div><p>intermédiaire</p></div></li>
                  <li class="logiciels"><div><p>CSS</p></div><div>...........</div><div><p>intermédiaire</p></div></li>
                  <li class="logiciels"><div><p>Javascript</p></div><div>.........</div><div><p>débutant</p></div></li>
                  <li class="logiciels"><div><p>Vue.js</p></div><div>............</div><div><p>débutant</p></div></li>
                  <li class="logiciels"><div><p>Node</p></div><div>............</div><div><p>débutant</p></div></li>
                </ul>

            </div>
            <div>
                <h1 class="titreCompetences">Compétences</h1>
                <ul>
                  <li><p>Curieuse</p></li>
                  <li><p>Créative</p></li>
                  <li><p>Flexible</p></li>
                  <li><p>Esprit d'equipe</p></li>
                  <li><p>Empathique</p></li>
                  <li><p>Professionnelle</p></li>
                </ul>

            </div>
            <div id="loisirs">
                <h1>Loisirs</h1>
                <div class="icon">
                    <i class="fas fa-palette"></i></div>
                <div class="icon">
                    <i class="fas fa-music"></i></div>
                <div class="icon">
                    <i class="fas fa-plane"></i></div>
                <div class="icon">
                    <i class="fas fa-glass-cheers"></i></div>
            </div>

        </aside>

    </div>

</template>

<script>
// @ is an alias to /src

export default {
  name: 'CV',
  components: {
    
  }
}
</script>

<style lang="scss">

@import "../sass/main.scss";



#cv{
    max-width: 980px;
    margin: auto;
    display: flex;
    // border: #5c6266 solid 1px;
    box-shadow: 3px 1px 10px $thirdColor;
    p{
      font-family: $serif;
    }
}


#headerCv{
  animation: none;
  left: 0;
}





/* aside*/

#photoIdentiteIdentite{
    width: 100%;
    text-align: center;
    margin-top: 13%;
}

#photoIdentiteIdentite img{
    width: 77%;
}

#photoIdentiteIdentite p{
    text-align: center;
}

aside{
    width: 30%;
    background: linear-gradient(to top, $quatreColor, 20%, $secondColor);
    position: relative;
    order: 1;

    img{
    width: 80%;
    height: 160px;
    border-radius: 50%; 
    margin-top: 15%;
    margin-left: 10%;
    }
    ul{
      padding-left: 10%;
      padding-right: 10%;
    }
    li{
      list-style: none;
      padding-left: 0;
    }
    .logiciels{
      width: 100%;
      display: flex;
      flex-direction: row;
      justify-content: space-between;
    }
}


.contenuContact {
    width: 90%;
    background-color: #fff;
    margin: auto;
    height: 130px;
    box-shadow: 3px 1px 10px $thirdColor;
    padding: 2%
    }

aside p{
    color:$firstColor;
    text-align: justify;
    line-height: 1.4rem;
    font-size:0.8rem;
    font-weight: 500;
}


aside h1{
    background-color: $firstColor;
    text-align: center;
    color: $secondColor;
    font-size: 1.4em;
    font-family: $serif;
    height: 29px;
    padding-bottom: 3px;
    margin-bottom: 20px;
    margin-top: 40px;
    &.titreLogiciels{
          height: 92px;
    }
}

a{
    text-decoration: none;
    color: $firstColor;
}

#loisirs{
    width: 100%;
    text-align: center;
    position: absolute;
    bottom: 20px;
}


#loisirs .fas{
    color: #fff;
    font-size: 1.3em;
}

.icon{
    display: inline-block;
    border: #fff solid 1px;
    border-radius: 30px;
    width: 35px;
    height: 35px;
    box-sizing: border-box;
    text-align: center;
    padding-top: 7px;
    margin-left: 4px;
    margin-right: 4px;

}
/*section*/


.contenuCv{
    box-sizing: border-box;
    width: 70%;
    padding-left: 3%;
    padding-right: 3%;
    order: 2;
    animation: none;
    p{
            line-height: 1rem;
                  font-size: 0.8rem;

    }
    
}

/*entete identité*/

.contenuCv header{
    margin-bottom: 25%;
    margin-top: 4%;
}

.contenuCv header h1{
    font-family: $serif;
    font-size: 3em;
    font-weight: 100;
    margin-bottom: 0;
}

.contenuCv header h2{
    font-size: 1.5rem;
    font-family: $serif;
    margin-top: 0;
    margin-bottom: 3px;
    font-weight: 300;
            .esperluette {
            font-size: 2rem;
            font-weight: 400;
            text-align: left;
            max-width: 980px;
            margin: auto;
            color: $secondColor;
        }
}
.contenuCv #layus{
    margin-top: 6%;
    p{
      font-size: 0.8rem;
      font-family: $serif;
    }
}

#julie{
    color:$secondColor;
    font-family: $serif;
    font-weight: 900;

}

#souligne{
    text-decoration: underline $secondColor;
    text-underline-position: under;
}

#filet{
    width: 26%;
    background-color: $secondColor;
    height: 2px;
}

/* bloc formation*/

article{
    width: 90%;
    margin-bottom: 15%;
    &.recommandation{
      margin-bottom: 3%;
    }
    
}

.bloc_section .fas{
    font-size: 2em;
    color: $thirdColor;
    position: absolute;
    bottom: 3px;
}

.titre{
    border-bottom: solid 2px $secondColor;
    margin-bottom: 30px;
    margin-top: 30px;
    position: relative;
    display: flex;


}

.titre h2{
    font-family: $serif;
    color:$firstColor;
    font-size: 1.6rem;
    margin-bottom: 0.2em;
    position: absolute;
    bottom: 0px;
    left: 55px;
    font-weight: 200;
}


.ligne{
    display: flex;
}

.ligne_collegue{
    display: flex;
}

.dates{
    width: 33%;
    display: flex;
    margin-right: 6%;
}

.dates .far{
    color: $secondColor;
    font-size: 0.8em;
    margin-right: 5px;
    line-height: 1.3em;
}

.dates .fas{
    color: $secondColor;
    font-size: 0.5em;
    margin-right: 10px;
    line-height: 2.8em;
    position: relative;
}



.contenu{
    width: 66%;
}

.contenu h5{
    font-size: 0.9rem;
    font-family: $serif;
    font-weight: 700;
    margin-top: 0;
    margin-bottom: 0.2em;
    color: $quatreColor;
}

.ligne{
    margin-bottom: 5px;
}

.ligne p{
    font-family: $serif;
    margin-top: 0;
    margin-bottom: 0;
    font-size: 0.8rem;
}

// .ligne_collegue{
//     margin-bottom: 35px;
// }

.ligne_collegue p{
    font-family: $serif;
    margin-top: 0;
    margin-bottom: 0;
}

.collegue{
    width: 50%;
}

.collegue h5{
    font-size: 0.9rem;
    font-family: $serif;
    margin-top: 0;
    margin-bottom: 0.2em;
    color: $quatreColor;
}

.collegue a{
    text-decoration: none;
    color:$firstColor;
}


/*image uniquement petit format*/
.contenuCv #identite_petit{
    display: none;
}


/*responsive tablettes*/

@media all and (min-width : 570px) and (max-width:768px){

    aside h1{
        height: auto;
    }

    article{
        margin-bottom: 25%;
    }

    article.bloc_section:last-child{
        margin-bottom: 0%;
    }


    .ligne{
        display: block;
    }

    .titre{
        margin-bottom: 5%;
        margin-top: 15%;
    }

    .dates{
        width: 100%;
    }

    .contenu{
        width: 100%;
        padding-left: 4%;
        margin-top: 1%;
    }

    .ligne_collegue{
        display: flex;
    }

    .icon {
        
        padding-top: 10px;
        margin-left: 2px;
        margin-right: 2px;
        margin-top: 15px;
    }

  
}




/*responsive mobiles*/

@media all and (max-width : 570px){

    #wrap{
        display: block;
    }

    p{
        font-size: 1em;
    }

    .contenuCv{
        order: 1;
        width: 100%;
        padding-left: 0%;
    }


    .contenuCv header{
        
        padding-top: 5%;
        padding-bottom: 5%;
        margin: 0%;
        display: flex;
        background-color: $secondColor;
    }

    .contenuCv header h1, h2{
        color: #ffffff;
    }

    #julie{
        color: $firstColor;
    }

    #filet{
        background-color: $firstColor;
    }

    .contenuCv #identite_petit{
        display: block;
        width: 30%;
        margin-right: 5%;
        margin-left: 5%;
        margin-top: 0%;
    }

    .contenuCv #identite{
        width: 60%;
    }

    .contenuCv #identite_petit img{
        width: 100%;
    }

    .contenuCv header h1 {
        font-family: $serif;
        font-size: 2.3em;
        font-weight: 100;
        margin-bottom: 0;
        margin-top: 3%;
    }

    article{
        padding-left: 3%;
        margin-bottom: 25%;
    }

    .titre {
        margin-bottom: 5%;
        margin-top: 15%;
    }
   

    .ligne{
        display: block;
        margin-bottom: 10%;
    }

    .ligne_collegue{
        display: block;
        // margin-bottom: 10%;
    }

    .contenu{
        margin-top: 1%;
        margin-left: 5%;
        width: 100%;
    }

    .contenu h2{
        color: #5c6266;
    }
    
    .dates{
        width:100% ;
    }

    .dates p{
        color: $secondColor;
    }

    
    
    .collegue{
        margin-bottom: 10%;
    }

    .collegue h5{
        color: $quatreColor;
    }


    aside{
        width: 100%;
        order: 2;
    }

    aside #photoIdentite{
        display: none;
    }

    #loisirs{
        position: relative;
    }



}



</style>
