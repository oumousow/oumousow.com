<template>
  <div class="container">
    <div class="card-container">
      <div class="card">
        <img :src="fiche.image" alt="Avatar">
        <div class="biography">
          <h4><b>{{ fiche.name }}</b>&nbsp;<em>({{ fiche.age }})</em></h4><br/>
          <p>{{ fiche.biography }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import FicheCard from "../fiche/FicheCard";

  export default {
    components: {FicheCard},
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
