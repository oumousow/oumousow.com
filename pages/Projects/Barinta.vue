<template>
<div>
  <div class="barinta">
  
      <p>Barinta est une jeune association fondée en juin 2017 et qui soutient l’éducation en Afrique principalement au Mali.
      Notre objectif est de donner aux jeunes évoluant dans les milieux défavorisés politiquement, socialement et économiquement une chance de réussite à l’école. Pour cela, nous leur fournissons des fournitures scolaires pour réunir un minimum de conditions favorisant une réussite scolaire et nous réalisons également des travaux de rénovation des matériels mobiliers et immobiliers.
Étant en Europe et eux en Afrique, nous leur offrons aussi une ouverture socioculturelle. Nous organisons des voyages humanitaires avec des bénévoles pour la distribution des matériels scolaires. Une fois sur le chantier, nous organisons aussi des activités culturelles afin de sensibiliser les jeunes sur l’importance des études avant la remise des matériels.
L’autre partie du projet consiste à instaurer un comité de suivi dans chaque établissement qui bénéficiera du projet afin de nous aider à évaluer l’envergure de nos actions et surtout pouvoir améliorer nos interventions et cibler les véritables besoins de ces établissements démunis. 
Pour mieux cibler les établissements et pouvoir les aider, nous avons mis en place une plateforme (https://kalanso.barinta.org/) sur laquelle vous pouvez retrouver une grande partie des écoles de différentes natures du Mali. 
Sur cette plateforme, apparaissent les noms de différentes écoles et nous invitons le public à compléter les informations manquantes s’il leur arrive de reconnaître leurs écoles. 
</p>  

<div>
    <b-carousel id="carousel1"
                style="text-shadow: 1px 1px 2px #333;"
                controls
                indicators
                background="#ababab"
                :interval="4000"
                img-width="1000"
                img-height="400"
                v-model="slide"
                @sliding-start="onSlideStart"
                @sliding-end="onSlideEnd"
    >

      <!-- Text slides with image -->
      <b-carousel-slide caption="First slide"
                        text="Fournitures offerts aux enfants"
                        :img-src="image3" img-alt="image3"></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide :img-src="image2" img-alt="image2">
        <h1>Fournitures offerts aux enfants</h1>
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide :img-src="image4" img-alt="image4">
      <h1>Photo souvenir avec les enfants</h1>
      </b-carousel-slide>

      <!-- Slides with img slot -->
      <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
      <b-carousel-slide>
        <img slot="img" class="d-block img-fluid w-100" width="1024" height="480"
             :src="image5" alt="image slot">
             <h1>Squetch enfants</h1>
      </b-carousel-slide>

      <!-- Slide with blank fluid image to maintain slide aspect ratio -->
      <!--  <b-carousel-slide :img-src="image6">
        <h1>Discours des enfants</h1>
        </b-carousel-slide> 
      -->
       <b-carousel-slide :img-src="image7" img-alt="image7">
        <h1>Discours des enfants</h1>
        </b-carousel-slide> 

         <b-carousel-slide :img-src="image8" img-alt="image8">
        <h1>Discours des enfants</h1>
        </b-carousel-slide> 

         <b-carousel-slide :img-src="image9" img-alt="image9">
        <h1>Discours des enfants</h1>
        </b-carousel-slide> 

         <b-carousel-slide :img-src="image10" img-alt="image10">
        <h1>Discours des enfants</h1>
        </b-carousel-slide> 

  <!--     <b-carousel-slide>
        <img slot="img" class="d-block img-fluid w-100" width="1024" height="480"
             :src="image11" alt="image slot">
             <h1>Squetch enfants</h1>
        </b-carousel-slide>
-->
         <b-carousel-slide :img-src="image12" img-alt="image12">
        <h1>Discours des enfants</h1>
        </b-carousel-slide> 

         <b-carousel-slide :img-src="image13" img-alt="image13">
        <h1>Discours des enfants</h1>
        </b-carousel-slide> 

         <b-carousel-slide :img-src="image15" img-alt="image15">
        <h1>Discours des enfants</h1>
        </b-carousel-slide> 

         <b-carousel-slide :img-src="image16" img-alt="image16">
        <h1>Discours des enfants</h1>
        </b-carousel-slide> 

      <b-carousel-slide caption="Blank Image" img-blank img-alt="Blank image">
      </b-carousel-slide>
    </b-carousel>

    <p class="mt-4">
      Slide #: {{ slide }}<br>
      Sliding: {{ sliding }}
    </p>

  </div>
  <div class="bouton">
      <a href="https://www.barinta.org"><b-button variant="primary">site</b-button></a>
  </div> 
  </div>
  </div>
</template>

<script>
import image3 from '../../assets/image3.jpg';
import image2 from '../../assets/image2.jpg';
import image4 from '../../assets/image4.jpg';
import image5 from '../../assets/image5.jpg';
import image7 from '../../assets/image7.jpg';
import image8 from '../../assets/image8.jpg';
import image9 from '../../assets/image9.jpg';
import image10 from '../../assets/image10.jpg';
import image12 from '../../assets/image12.jpg';
import image13 from '../../assets/image13.jpg';
import image15 from '../../assets/image15.jpg';
import image16 from '../../assets/image16.jpg';

export default {
  name:'barinta',
  components: {
 
  },
  data () {
    return {
      slide: 0,
      sliding: null,
      image3: image3,
      image2: image2,
      image4: image4,
      image5: image5,
      image7: image7,
      image8: image8,
      image9: image9,
      image10: image10,
      image12: image12,
      image13: image13,
      image15: image15,
      image16: image16,
     
    }
  },
  methods: {
    onSlideStart (slide) {
      this.sliding = true
    },
    onSlideEnd (slide) {
      this.sliding = false
    }
  }  
}
</script>

<style>
.barinta
{
  background-color: white;
  padding-left: 30px;
  padding-right: 30px;
  padding-top: 10px;
}
.bouton
{
padding-left:600px;
margin-left: 55px;
}
</style>
