<template>
<div>
<div class="projets"> 
<!--<HelloWorld msg="Welcome to Your Vue.js App"/>-->
<!--
<div class="card-group">
  <div class="card">
    <img src="../assets/Plume.jpg" class="card-img-top" alt="...">
    <div class="card-body">
      <h3 class="card-title">Écriture(Nouvelles)</h3>
      <p class="card-text">Dépuis 2016, j'écris des nouvelles, courtes et faciles à lire normalement :-).<br>
      <router-link to="/projects/ecriture"><b-button variant="primary">Suivre</b-button></router-link>
      </p>
    </div>
    <div class="card-footer">
      <small class="text-muted">Last updated 3 mins ago</small>
    </div>
  </div>

  <div class="card">
    <img src="../assets/pl.png" class="card-img-top" alt="https://www.barinta.org">
    <div class="card-body">
      <h3 class="card-title">Association Barinta</h3>
      <p class="card-text">Barinta est une association fondée en 2017 par <a href="https://www.linkedin.com/in/cheick-mahady-sissoko-45482b63/">Cheick Mahady Sissoko </a> 
      et moi même.<br> Ella a pour objetif de soutenir l'éducation des enfants dans les zones défavorisées de l'Afrique de l'Ouest.<br>
      <router-link to="/projects/barinta"><b-button variant="primary">En savoir plus</b-button></router-link>
     </p>
    </div>
    <div class="card-footer">
      <small class="text-muted">Last updated 3 mins ago</small>
    </div>
  </div>

  <div class="card">
    <img src="../assets/innovafrq.jpg" class="card-img-top" alt="...">
    <div class="card-body">
      <h3 class="card-title">Plan d'Action Pour l'Afrique</h3>
      <p class="card-text">L'Afrique est probablement le continent le plus riche en terme de matières premières dans le monde.<br>Alors pourquoi est-elle la plus sous-développée?<br>Qu'avons-nous à apporter en tant que jeunes?<br>
      <router-link to="/projects/paa"><b-button variant="primary">En savoir plus</b-button></router-link>
      </p>
    </div>
    <div class="card-footer">
      <small class="text-muted">Last updated 3 mins ago</small>
    </div>
  </div>
</div>
-->

<div>
    <b-card-group deck>
      
        <b-card title="Association Barinta"
                :img-src="pl"
                img-alt="Img"
                img-top>
             <div class="ordre"> 
            <p class="card-text">Barinta est une association fondée en 2017 par <a href="https://www.linkedin.com/in/cheick-mahady-sissoko-45482b63/">Cheick Mahady Sissoko </a> 
      et moi même.<br> Ella a pour objetif de soutenir l'éducation des enfants dans les zones défavorisées de l'Afrique de l'Ouest.<br>
     </p>
             </div>
            <div slot="footer">
                <router-link to="/projects/barinta"><b-button variant="primary">En savoir plus</b-button></router-link>
                <small class="text-muted">Last updated 3 mins ago</small>
            </div>
        </b-card>
        <b-card title="Écriture(Nouvelles)"
                :img-src="Plume"
                img-alt="Img"
                img-top>
            <div class="ordre">
            <p class="card-text">Dépuis 2016, j'écris des nouvelles, courtes et faciles à lire normalement :-).<br>
            </p>
            </div>
            <div slot="footer">
                <router-link to="/projects/ecriture"><b-button variant="primary">En savoir plus</b-button></router-link>
                <small class="text-muted">Last updated 3 mins ago</small>
            </div>
            
        </b-card>
        <b-card title="Plan d'Action Pour l'Afrique"
                :img-src="innovafrq"
                img-alt="Img"
                img-top>
            <p class="card-text">L'Afrique est probablement le continent le plus riche en terme de matières premières dans le monde.<br>Alors pourquoi est-elle la plus sous-développée?<br>Qu'avons-nous à apporter en tant que jeunes?<br>
      
           </p>
            <div slot="footer">
                <router-link to="/projects/paa"><b-button variant="primary">En savoir plus</b-button></router-link>
                <small class="text-muted">Last updated 3 mins ago</small>
            </div>
        </b-card>
    </b-card-group>
</div>

</div>
</div>
</template>

<script>
import pl from '../assets/pl.png';
import Plume from '../assets/Plume.jpg';
import innovafrq from '../assets/innovafrq.jpg';
export default {
name:'projets',
components: 
{
 
},
data (){
  return{
    pl:pl,
    Plume:Plume,
    innovafrq:innovafrq,
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