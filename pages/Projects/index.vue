<template>
  <div class="body">
     <strong class="def"> Mes projets </strong>
    <project-list :projects="projects"></project-list>
  </div>
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
 margin: 600px;
 margin-top: 100px;
}
</style>
