<template>
  <div class="body">
    <project-detail :project="project" ></project-detail>
  </div>
</template>

<script>
  import ProjectDetail from "../../../components/project/ProjectDetail";
  import data from "../../../data/projects.json"

  export default {
    components: {ProjectDetail},
    asyncData(context) {
      return {
        project: data.find(project => project.id === context.params.title)
      }
    }
  }
</script>
