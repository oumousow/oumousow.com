<template>
  <nuxt-link :to="redirection">
    <div>
   
    </div>
    <div class="card">
    </div>
  </nuxt-link>
</template>

<script>
  export default {
    props: {
      fiche: {
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
    height: 15rem;
    width: 13rem;
    overflow: hidden;
    margin: auto;
  }

  .card {
    padding: .5rem;
  }
  a, a:hover {
    text-decoration : none !important;
    color: black !important;
    }
   
</style>
