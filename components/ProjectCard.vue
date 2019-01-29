<template>
    <b-card :title="project.title" :img-src="project.image" img-alt="Img">
        <p class="card-text">{{ project.description }}</p>
        <div slot="footer">
            <router-link to="/projects/paa">
            <b-button variant="primary">En savoir plus</b-button></router-link>
        </div>
    </b-card>
</template>

<script>
  export default {
    props: {
      project: {
        type: Object,
        default: () => {}
      },
      redirection: {
        type: String,
        default: () => ''
      }
    }
  }
</script>

<style scoped>
  .media {
    height: 20rem;
    overflow: hidden;
  }

  .card {
    padding: .2rem;
  }
</style>