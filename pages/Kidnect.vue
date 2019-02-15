<template>
<div>
   
<div class="content">
<section id="mysect1">

 <b-card title=""
                :img-src="kidnect"
                img-alt="Img"
                img-top>
            <p class="card-text">
                Nous vous proposons dans un moyen de sortir en Famille en évitant de porter atteinte à votre sérénité :<strong> KIDNECT </strong>. Je suis sure que durant les moments de sorties tout le monde souhaiterait pouvoir laisser les enfants faire ce qu’il veulent de manière autonome sans s’inquieter de savoir comment les retrouver après.
            <div slot="footer">
                <small class="text-muted">Last updated 3 mins ago</small>
            </div>
        </b-card>

</section>
<section id="mysect2">
    <b-card
:img-src="watcher0"
                img-alt="Img"
                img-top>
            <p class="card-text">
                <strong> KIDNECT </strong> est un dispositif qui vous permet de garder un œil sur vos enfants lors de vos sorties en grandes surfaces comme au parc d’attraction et autres lieux ludiques attirants beaucoup de monde. Grâce à Watcher vous pouvez savoir où se trouve vos enfants à tout moment en envoyant un simple message au dispositif que portera l’enfant. De son côté il pourra lui aussi vous communiquer sa position en appuyant sur un simple bouton.Avec KIDNECT Changez votre expérience des sorties en famille </p>
            <div slot="footer">
                <small class="text-muted">Last updated 3 mins ago</small>
            </div>
        </b-card>
        
</section>
<section id="mysect3">
<h1>SECTION 3</h1>
</section>
<section id="mysect4">
<h1>SECTION 4</h1>
</section>
<section id="mysect5">
<h1>SECTION 5</h1>
</section>
<section id="mysect6">
<h1>SECTION 6</h1>
</section>
</div>

<!-- Start vertical navigation -->
<div id="op-verticalnav">
<ul class="op-sectionlist">
<li class="op-v-item"><a class="op-v-link" href="#mysect1"><span class="v-marker"></span><span class="op-v-itemdesc"><span class="op-v-itembg">Naviguer vers la section 1</span></span></a></li>
<li class="op-v-item"><a class="op-v-link" href="#mysect2"><span class="v-marker"></span><span class="op-v-itemdesc"><span class="op-v-itembg">Lire la section 2</span></span></a></li>
<li class="op-v-item"><a class="op-v-link" href="#mysect3"><span class="v-marker"></span><span class="op-v-itemdesc"><span class="op-v-itembg">Directement à la section 3</span></span></a></li>
<li class="op-v-item"><a class="op-v-link" href="#mysect4"><span class="v-marker"></span><span class="op-v-itemdesc"><span class="op-v-itembg">Se rendre à la section 4</span></span></a></li>
<li class="op-v-item"><a class="op-v-link" href="#mysect5"><span class="v-marker"></span><span class="op-v-itemdesc"><span class="op-v-itembg">Voir la section 5</span></span></a></li>
<li class="op-v-item"><a class="op-v-link" href="#mysect6"><span class="v-marker"></span><span class="op-v-itemdesc"><span class="op-v-itembg">Dernière section de la page</span></span></a></li>
</ul>
</div>
<!-- end vertical navigation -->



</div>
</template>


<script>
import kidnect from '../assets/kidnect.png';
import watcher0 from '../assets/watcher0.png';
import watcher1 from '../assets/watcher1.png';
export default {
data () {
    return {
      slide: 0,
      sliding: null,
      kidnect:kidnect,
      watcher0:watcher0,
}
}
}
</script>


<style>
#op-horizontalnav {background:#171717; position:fixed; top:0; right:0; left:0}
#op-horizontalnav .op-sectionlist {width:100%; max-width:1280px; margin:auto;padding:0; text-align:center; display:table;}
#op-horizontalnav .op-v-item {list-style:none; display:table-cell; font-size:16px}
#op-horizontalnav .op-v-item .op-v-link {color:#fff; padding:16px 8px;display:block;text-decoration:none}
#op-horizontalnav .op-v-item .op-v-link:hover, #op-horizontalnav .op-v-link.active {background-color:#fff;color:#171717}

section h1 {padding:450px; text-align:initial ; color:black; background:rgb(236, 226, 226); border-top:1px solid red; margin:0}
section:nth-child(even) h1 {background:white;} /*on différencie la couleur 1 section sur 2*/


#op-verticalnav {position:fixed; top:0; right:0; left: auto;height: 100%;display:table}
#op-verticalnav .op-sectionlist {height:100%; text-align:center; display:table-cell; vertical-align:middle}
#op-verticalnav .op-v-item {display:block}
#op-verticalnav .justify-height {}
#op-verticalnav .op-v-link {display:block; margin:12px 0}
#op-verticalnav .v-marker {width:15px; height:15px; border-radius:50%; background-color:rgba(255,0,27,.4); display:inline-block; vertical-align:middle; margin-bottom:-2px; margin-right:10px;border: 1px solid #e1001b;}
#op-verticalnav .op-v-link:hover .v-marker, #op-verticalnav .op-v-item .op-v-link.active .v-marker {background-color:rgba(255,0,27,1); }
#op-verticalnav .op-v-itemdesc {display:inline-block; font-size:14px; position:absolute; white-space:nowrap; line-height:normal; padding:0 34px 0 0;vertical-align:middle}
#op-verticalnav .op-v-itemdesc .op-v-itembg{display:inline-block; background-color:rgba(0,0,0,.5); color:#fff; padding:4px 10px 6px 10px; border:1px solid rgba(160,160,160,.2); border-radius:4px; }
#op-verticalnav .op-v-link:hover .op-v-itemdesc {right:0px; }
.card-img-top {
    width: 60%;
    margin-left: 250px;
}
</style>
