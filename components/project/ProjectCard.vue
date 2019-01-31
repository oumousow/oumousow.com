<template>
<div class="corps">
    <nuxt-link :to="redirection">
      <div class="media">
        <img :src="project.image" alt="Avatar" style="width: 100%">
      </div>
      <div class="card">
        <div>
          <h4><b>{{ project.title }}</b>&nbsp;<em>({{ project.year }})</em></h4>
          <p>{{ project.description }}</p>
        </div>
      </div>
    </nuxt-link>
</div>    
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

<style type="css" scoped>
  .corps
  {
    padding-left: 10px;
  }
  
  .media {
    height: 20rem;
    overflow: hidden;
  }

  .card {
    padding: .5rem;
  }

  .card p {
      text-decoration : none !important;
    }

    a, a:hover {
    text-decoration : none !important;
    color: black !important;
    
    }
</style>




















<!--
<template class="regle">

    <b-card :title="project.title" :img-src="project.image" img-alt="Img" >
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
    min-height: 37rem;
  }
 
  
</style>
-->