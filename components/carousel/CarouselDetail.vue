<template>
  <div class="container">
  <div>
    <b-carousel id="carousel1"
                style="text-shadow: 1px 1px 2px #333;"
                controls
                indicators
                background="#ababab"
                interval="4000"
                img-width="1000"
                img-height="400"
                v-model="slide"
                @sliding-start="onSlideStart"
                @sliding-end="onSlideEnd">
      <b-carousel-slide caption="First slide"
                        :text="carousel.descrip"
                        :img-src="carousel.images" img-alt="image3">
      </b-carousel-slide>
      </b-carousel>
        </div>
      </div>
</template>

<script>
  import CarouselCard from "../carousel/CarouselCard";
 

  export default {
    components: 
    {
        FicheCard,
      
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
