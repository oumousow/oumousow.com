<template>

<div class="corps">
    <nuxt-link :to="redirection">
      <div class="media">
        <h4><b>{{ project.title }}</b></h4><br><br><br><br> <br>
        <img :src="project.image" alt="Avatar" style="width: 100%">
      </div>
      <div class="card">
        <div>
          <p>{{ project.description }}</p>
        </div>
         <br> <br> <br>
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
    margin-top: 1px;
    margin-right: 3px;
    margin-left: -7px;
    border-radius: 1.25rem;
    max-width: 314px;
    height: 176px;
}
  .card p {
      text-decoration : none !important;
    }

    a, a:hover {
    text-decoration : none !important;
    color: black !important;

    }
    img {
    vertical-align: middle;
    max-width: 300px;
    height: 240px;
    margin-left: -72px;
    margin-top: 70px;

}
.card {
    position: relative;
    display: flex;
    flex-direction: column;
    min-width: 0;
    word-wrap: break-word;
    background-clip: border-box;
    border: 1px solid rgb(255, 255, 255);
    border-radius: 0.25rem;
}
h4, .h4 {
    font-size: 1.2rem;
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