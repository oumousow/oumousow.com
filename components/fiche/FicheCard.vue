<template>
  <nuxt-link :to="redirection">
    <div class="media">
      <img :src="fiche.image" alt="Avatar" style="width: 100% ">
    </div>
    <div class="card">
      <div>
        <h4><b>{{ fiche.name }}</b>&nbsp;<em>({{ fiche.age }})</em></h4>
      </div>
    
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
    height: 14rem;
    width: 13rem;
    overflow: hidden;
    margin: auto;
  }

  .card {
    padding: .5rem;
    max-width: 266px;
    margin: 12px;
    height: 68px;
  }
  a, a:hover {
    text-decoration : none !important;
    color: black !important;
    }
     img {
    margin-top:20px;
    vertical-align: top;
    border-style: none;
    max-width: 209px;
    height: 200px;
}
</style>
