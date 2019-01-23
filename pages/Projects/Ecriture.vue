<template>
<div>
 
 <div class='ecriture'>
  <div>
    <b-card-group deck>
        <b-card header="Oumou Sow"
                header-tag="header"
                footer="Premier prix écriture Achères"
                footer-tag="footer"
                title="De l'autre coté">
            <p class="card-text">c'est une nouvelle qui a emporté le premier prix du concours d'achères en 2016. </p>
            <p class="card-text">La nouvelle parle d'un jeune homme qui part faire ces études en France et qui découvre un nouveau monde où sa vie va totalement changer</p>
           
           <router-link to="/projects/Brinta"> <b-button variant="primary">lire</b-button> </router-link>
        </b-card>
        <b-card title="Title"
                header-tag="header"
                footer-tag="footer">
            <h6 slot="header"
                class="mb-0">Header Slot</h6>
            <em slot="footer">Footer Slot</em>
            <p class="card-text">Header and footers using slots.</p>
            <b-button variant="primary">Go somewhere</b-button>
        </b-card>
    </b-card-group>
</div>
 </div> 
</div> 
</template>

<script>
import Nav from '@/components/Nav.vue'
export default {
    
   name:'ecriture',
components: 
{

}
}
</script>


<style>
  
</style>