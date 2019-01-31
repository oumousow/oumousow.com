<template>
  <div class="body">
    <fiche-detail :fiche="fiche"></fiche-detail>
  </div>
</template>
<script>
  import FicheDetail from "../../../components/fiche/FicheDetail";
  import data from "../../../data/projects.json"

  export default {
    components: {FicheDetail},
    asyncData({ params }) {
      return {
        fiche: data.find(project => project.id === params.title).casting.find(fiche => fiche.id === params.fiche)
      }
    }
  }
</script>
