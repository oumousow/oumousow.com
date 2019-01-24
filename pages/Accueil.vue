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
            I start opened because <code>visible</code> is <code>true</code>
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
        Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry
        richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor
        brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon
        tempor, sunt aliqua put a bird on it squid single-origin coffee nulla
        assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore
        wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher
        vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic
        synth nesciunt you probably haven't heard of them accusamus labore VHS.
      `,
      msg:
      
      `
Adja, je suis en satge chez Mobennnn 

      `,
      sms:
      `
        lmkf    jphgbn  fjh bifegvç oefja^rué'yàtg  uobzpfijhobutg!àhzçv jytyéà'!çru^yg"g!à     !tg tçè!    'yrpojmgheripg

      `,
      mes:
      `
        afjpzruog   !rp&u"rày!éhruogjoz^g   !y""ç!téji  bgug    çè"ty!àtjgbkgiyeg!"èty'ç"(gt hogohgipketho!qçèytepçgojrnmkbb " y!tphot)

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
