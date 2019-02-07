<template>
  <div class="home">
    <b-row>
      <b-col md="12">
        <section class="text-center mt-5">
          <h1>
            Bienvenue sur mon site 
          </h1>
          <p class="welcome">
            Merci à <a href="https://nouhoumtraore.co">Nouhoum Traoré </a> et à toute son <a href="https://www.linkedin.com/company/moben-technology/about/">équipe</a>
          </p>
      </section>
      </b-col>
</b-row>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  layout: 'home-layout',
  components: {
    Logo
  }
}
</script>

<style>
.home {
  color: #ffffff;
  z-index: 2;
  margin-top:27%;
  top:0;
  position: absolute;
  width: 100%;
  text-align: center;
}

.welcome   {
  font-size: 1.2rem;
}
</style>
