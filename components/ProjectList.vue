<template>
  <div class="container">
    <section class="list">
      <div class="card-container" v-for="project in projects" :key="project.id">
        <project-card :project="project"></project-card>
      </div>
    </section>
  </div>
</template>

<script>
  import ProjectCard from "../components/ProjectCard";

  export default {
    components: {ProjectCard},
    props: {
      projects: {
        type: Array,
        default: () => []
      }
    }
  }
</script>

<style scoped>
  .container {
    margin-top: 3rem;
  }

  .card-container {
    width: 20rem;
    height: 36rem;
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
    cursor: pointer;
  }

  .card-container:hover {
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.5);
  }

  .list {
    display: grid;
    flex-direction: row;
    grid-gap: 5rem;
    grid-template-columns: auto auto auto;
    padding-left: 7rem;
  }
</style>