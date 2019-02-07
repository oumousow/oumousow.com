<template> 
  <div class="bg-container" >
     <div class="bg-img">
    </div>
    <Nav/>
    <nuxt />
  </div>
</template>

<style>
html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Source Sans Pro',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.bg-container {
  background: url("../assets/image1.png");
  background-position: center top;
  background-size: cover;
}
.bg {
  width: 100%;
  position: absolute;
  z-index: 0;
  
  top: 0;
  bottom: 0;
  background-color: hsla(239, 100%, 50%, 0.47);
}

.bg img {
  width: 100%;
  background-color: hsla(239, 100%, 50%, 0.47);
}

.bg-img {
  z-index: 1;
  height: 100vh;
  width: 100%;
  top: 0;
  bottom: 0;
  background-color: hsla(239, 100%, 50%, 0.47);
}
.bg-container  .bar {
  z-index: 2;
  position: absolute;
  top: 0;
  width: 100%;
  border-bottom: none;  
}

.bg-container  nav.navbar {
  background-color: transparent !important;
  color: #ffffff;
}

.bg-container .nav-link  {
  color: #ffffff !important;
}
</style>

<script>
import Nav from '@/components/Nav'
export default {
  components: { Nav }
}
</script>

