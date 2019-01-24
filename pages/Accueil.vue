<template>
<div class="accueil">
  <section class="container">
    <div>
      <h3 class="title">
        Mon stage chez Moben Technologie/<br>Figaro-classifieds
      </h3>
      <h5 class="subtitle">
<p>Mon stage chez Moben Technology s’est déroulé essentiellement au tour du sujet :</p>
   <p><strong> "Comment aider  les chercheur d’emploi à trouver du travail facilement?"</strong><p>
<p>Pour cela j’étais immergée durant mes six semaines de stages au sein de l’équipe de Keljob chez Figaro-Classifieds.</p>
      </h5>  
  <div role="tablist">
    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-btn block href="#" v-b-toggle.accordion1 variant="info">Action 1</b-btn>
      </b-card-header>
      <b-collapse id="accordion1" visible accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <p class="card-text">
           <!-- I start opened because <code>visible</code> is <code>true</code>-->
          </p>
          <p class="card-text">
            {{ text }}
          </p>
        </b-card-body>
      </b-collapse>
    </b-card>
    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-btn block href="#" v-b-toggle.accordion2 variant="info">Action 2</b-btn>
      </b-card-header>
      <b-collapse id="accordion2" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <p class="card-text">
            {{ msg }}
          </p>
        </b-card-body>
      </b-collapse>
    </b-card>
    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-btn block href="#" v-b-toggle.accordion3 variant="info">Action 3</b-btn>
      </b-card-header>
      <b-collapse id="accordion3" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <p class="card-text">
            {{sms}}
          </p>
        </b-card-body>
      </b-collapse>
    </b-card>
    

    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-btn block href="#" v-b-toggle.accordion4 variant="info">Action 4</b-btn>
      </b-card-header>
      <b-collapse id="accordion4" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <p class="card-text">
            {{ mes }}
          </p>
        </b-card-body>
      </b-collapse>
    </b-card>

  </div>

    </div>
  </section>
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
.accueil
{
  background-color:rgba(0, 0, 0,0.6);
}
.container {
  margin: 0 auto;
  min-height: 93vh;
  display: flex;
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
  color:white;
  /* #35495e*/
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 250;
  font-size: 25px;
  color:white;
  /*#526488*/
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
