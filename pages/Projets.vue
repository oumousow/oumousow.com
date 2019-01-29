<template>
<div>
<div class="projets"> 
<div>
    <b-card-group deck>
          <project-list :projects="projects"></project-list>
    </b-card-group>
</div>
</div>
</div>
</template>

<script>
import pl from '../assets/pl.png';
import Plume from '../assets/Plume.jpg';
import innovafrq from '../assets/innovafrq.jpg';
import data from '../data/projects.json';
import ProjectList from '../components/ProjectList.vue'
export default {
name:'projets',
components: 
{
 ProjectList
},
data (){
  return{
    projects: data,
  }
}
}
</script>

<style>
.projets
{
  padding-left: 20px;
  padding-right: 20px;
  background-color: white;
}
.ordre
{
  padding-top: 50px;
}
</style>