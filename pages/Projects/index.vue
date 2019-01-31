<template>
  <div class="body">
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
</style>
