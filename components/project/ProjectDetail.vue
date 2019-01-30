<template>
  <div class="container">
    <div class="card-container">
      <div class="media">
        <img :src="project.cover" alt="Barinta" style="width: 100%">
      </div>
      <div class="card">
        <div>
          <h4><b>{{ project.title }}</b>&nbsp;<em>({{ project.year }})</em></h4>
          <p>{{ project.description }}</p>
          <div class="container">
            <h4>Casting</h4>
            <section class="actors">
              <div v-for="id in project.detail" :key="id.id" class="detail">
                <project-card :id="id" :redirection="`/films/${project.id}/${actor.id}`"></project-card>
              </div>
            </section>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import FicheCard from "../fiche/FicheCard";
  export default {
    components: {ficheCard},
    props: {
      movie: {
        type: Object,
        default: () => {
        }
      }
    }
  }
</script>

<style scoped>
  .media {
    height: 30rem;
    overflow: hidden;
  }
  .card {
    padding: 1rem 3rem 2rem 3rem;
  }
  .card-container {
    width: 60rem;
    height: 65rem;
    margin: auto;
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
  }
  .detail {
    display: grid;
    flex-direction: row;
    grid-gap: .5rem;
    grid-template-columns: auto auto auto;
    margin-top: 2rem;
    padding-left: 2.5rem;
  }
  .detail {
    margin: auto;
    cursor: pointer;
    text-align: center;
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
  }
  .detail:hover {
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.5);
  }
</style>