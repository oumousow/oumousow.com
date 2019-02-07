<template> 
  <div>
    <Nav/>
    <b-container>
      <nuxt />
    </b-container>
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

body {
  background-color: #fafafa;
}

p {
  line-height: 1.9rem;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

</style>

<script>
import Nav from '@/components/Nav'
export default {
  components: { Nav }
}
</script>

