<template>
  <div class="container">
    <div class="card-container">
      <div class="card">
        <img :src="fiche.image" alt="Avatar">
        <div class="biography">
          <h4><b>{{ fiche.name }}</b>&nbsp;<em>({{ fiche.age }})</em></h4><br/>
          <p>{{ fiche.biography }} <a href="https://www.barinta.org"> {{fiche.site}} </a></p>
        </div>
        <br><br>

              <div>
        
    <b-carousel id="carousel1"
                style="text-shadow: 1px 1px 2px #333;"
                controls
                indicators
                background="#ababab"
                :interval="4000"
                img-width="900"
                img-height="400"
                >
              <!--
                v-model="slide" 
                 @sliding-start="onSlideStart"
                @sliding-end="onSlideEnd"
                -->
      <b-carousel-slide 
      v-for="(image, key) in fiche.carousel.images"
      :key="key"
                        :text="image.description"
                        :img-src="image.url" img-alt="images">
      </b-carousel-slide>
      
      </b-carousel>
      </div>
      </div>
    </div>
  </div>
</template>

<script>
  import FicheCard from "../fiche/FicheCard";
 

  export default {
    components: 
    {
        FicheCard
    },
    props: {
      fiche: {
        type: Object,
        default: () => {
        }
      }
    }
  }
</script>

<style scoped>
  
  img {
    width: 13rem;
    
  }

  .container
  {
      background-color: white;
      max-width: 1437px;
  }
  /*.centre
  {
    padding-left: 200px;
  }
  */
  .biography {
    padding: 1rem 2rem;
  }

  .card {
    padding: 2rem 3rem 2rem 3rem;
    display: grid;
    grid-template-columns: auto auto;
    text-decoration: none;
  }

  .card-container {
    width: 70rem;
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
    margin: auto;
    display: grid;
    grid-template-columns: auto auto;
  }

</style>
