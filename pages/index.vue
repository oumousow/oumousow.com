<template>
<div class="effet">
  <section class="container">
    <div>
      <!--<logo />-->
      <h1 class="title">
        Oumou Sow
      </h1>
      <h2 class="subtitle">
        Bienvenue sur mon site 
      </h2>
      <h4 class="soustitre">
        Merci à <a href="https://nouhoumtraore.co">Nouhoum Traoré </a> et à toute son <a href="https://www.linkedin.com/company/moben-technology/about/">équipe</a>
      </h4>
    </div>
  </section>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.effet
{
  background-color:rgba(0, 0, 0, 0.8);
}
.container {
  margin: 0 auto;
  min-height: 93vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color:white;
  /* #35495e*/
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color:white;
  /*#526488*/
  word-spacing: 5px;
  padding-bottom: 15px;
}
.soustitre
{
   color:white;
  font-weight: 300;
  
}

.links {
  padding-top: 15px;
}
</style>
