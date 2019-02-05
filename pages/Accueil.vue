<template>
<div class="accueil">
  <div class="largeur">
  <section class="container">
    <div>
   <!--   <h4 class="title">
        Mon stage chez Moben Technologie/<br>Figaro-classifieds
      </h4>
      <h6 class="subtitle">
<p>Mon stage chez Moben Technology s’est déroulé essentiellement au tour du sujet :</p>
   <p><strong> "Comment aider  les chercheur d’emploi à trouver du travail facilement?"</strong><p>
<p>Pour cela j’étais immergée durant mes six semaines de stages au sein de l’équipe de Keljob chez Figaro-Classifieds. Et pour cela, il m'a fallu apprendre apprendre à faire du développement web grâce aux outils suivants.</p>
      </h6> --> 

  <div class="page1">
    <b-card  bg-variant="transparent"  text-variant="white"  title=" Mon stage chez Moben Technology-Figaro-classifieds"
            sub-title="">
 <div class="text1">    
<p>Mon stage chez Moben Technology s’est déroulé essentiellement au tour du sujet :</p>
   <p><strong> "Comment aider  les chercheur d’emploi à trouver du travail facilement?"</strong></p>
<p>Pour cela j’étais immergée durant mes six semaines de stages au sein de l’équipe de Keljob chez Figaro-Classifieds. Pour faire un site web, il faut connaitre les outils selon plusieurs étapes suivantes:</p>
</div>        
        <a href="https://moben.fr/"
           class="card-link">Moben Technology</a>
        <b-link href="https://www.keljob.com/"
                class="card-link">Keljob</b-link>
    </b-card>
</div>
 

<!-- 
<b-card  bg-variant="transparent" text-variant="white" title="Card Title">
  <p class="card-text">
    With supporting text below as a natural lead-in to additional content.
  </p>
  <b-button href="#" variant="primary">Go somewhere</b-button>
</b-card>
-->

  <div role="tablist">
    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-btn block href="#" v-b-toggle.accordion1 variant="info">Etape 1</b-btn>
      </b-card-header>
      <b-collapse id="accordion1" visible accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <p class="card-text">
           <!-- I start opened because <code>visible</code> is <code>true</code>-->
          </p>
          <p class="card-text">
            {{ text }}
          </p>
          <p class="card-text"> <router-link to="/accueil">suivre</router-link> </p>
        </b-card-body>
      </b-collapse>
    </b-card>
    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-btn block href="#" v-b-toggle.accordion2 variant="info">Etape 2</b-btn>
      </b-card-header>
      <b-collapse id="accordion2" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <p class="card-text">
            {{ msg }}
          </p>
          <p class="card-text"> <router-link to="/accueil">suivre</router-link> </p>
        </b-card-body>
      </b-collapse>
    </b-card>
    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-btn block href="#" v-b-toggle.accordion3 variant="info">Etape 3</b-btn>
      </b-card-header>
      <b-collapse id="accordion3" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <p class="card-text">
            {{sms}}
          </p>
          <p class="card-text"> <router-link to="/accueil">suivre</router-link> </p>
        </b-card-body>
      </b-collapse>
    </b-card>
    

    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-btn block href="#" v-b-toggle.accordion4 variant="info">Etape 4</b-btn>
      </b-card-header>
      <b-collapse id="accordion4" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <p class="card-text">
            {{ mes }}
          </p>
          <p class="card-text"> <router-link to="/accueil">suivre</router-link> </p>
        </b-card-body>
      </b-collapse>
    </b-card>

  </div>

    </div>
    <div class="flotte">
     <img src="../assets/babyboss2.png" width="150px" alt="Nouveau !" />
    </div>
  </section>
  </div>
  <!--<section class="flotte">
 <img src="../assets/babyboss2.png" width="70px" alt="Nouveau !" />
  </section>-->
  </div>
</template>


<script>
export default 
{  
  name: 'accueil',
 data () {
    return {
      text: `
        Html, css
      `,
      msg:
      
      `
Boostrap
      `,
      sms:
      `
Vue js, Boostrapsvue
      `,
      mes:
      `
Nuxt, Déployement sur Heruku via github
      `

    }
  }
}

</script>

<style>
.largeur
{
  padding-left: 10px;
  
}
.accueil
{
  background-color:rgba(0, 0, 0,0.6);
}
.container {
  /*margin: 10px;*/
  margin-right: 10px;
  margin-left: 160px;
  width: 100%;
  /**0 auto*/
  min-height: 93vh;
  display: flex;
  position:absolute;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
  'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 350;
  font-size: 60px;
  color:black;
  /* #35495e*/
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 250;
  font-size: 25px;
  color:black;
  /*#526488*/
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
.flotte
{
  float:left;
  padding: 0px;
  margin-top: 300px;
}
.page1
{
margin-left: 0px;
margin-right: 0px;
text-decoration-color: black;

}
.text1
{
  color: black;
 
}
</style>
