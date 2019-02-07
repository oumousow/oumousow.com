<template>
  <b-card title="Mes projets">
    <b-card-body>
      <project-list :projects="projects"></project-list>
    </b-card-body>
  </b-card>
</template>
<script>
  import ProjectList from "../../components/project/ProjectList";
  import data from "../../data/projects.json"

  export default {
    components: {ProjectList},
    data() {
      return {
        projects: data
      }
    }
  }
</script>

<style>
.body
{
  background-color: white;
}
.def
{
 margin: 530px;
 margin-top: 100px;
}
</style>
