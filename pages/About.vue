<template>
<div>
  <div class="about">
   
     <div>
    
     <b-card title="Qui suis-je?">
            <p class="card-text">

<p>
<strong>Présentation :</strong><br>

Je m’appelle Oumou Sow, je suis en école d’ingénieur à l’école Centrale d’Électronique de Paris ECE Paris-Lyon. 

    Je suis née au Sénégal et j’y ai grandi  jusqu’à mes 15 ans.  J’ai vécu dans ce que l’on appelle une famille typique Sénégalaise : mamie, papi, tata, tonton, cousin, cousine, le reste de la bande et la liste est très longue. 
    Cela m’a permis de développer un coté humanitaire très important et une ouverture d’esprit par rapport au monde qui m’entoure. 
</p><br>
<p>
<strong> Mes activités :</strong><br>

    Depuis 2016, je suis engagée dans différentes associations qui ont pour but de contribuer au développement de l’Afrique  à travers l’éducation, l’entreprenariat de la jeunesse africaine et la paix. 
    Dans ce cadre, j’ai coordonnée 3 ans le Forum FIND AFRICA (Forum International pour  le Développement de l’Afrique 2016-2019) pour l’association CRD (Cadre de Réflexion pour le Développement).
    Je suis actuellement la vice-présidente de l’association Barinta. Barinta œuvre pour donner aux enfants d’établissements démunis des endroits éloignés et défavorisés, une chance de réussir leurs études. Pour cela, elle choisit chaque année un établissement sur des critères établis par l’association et nous lui offrons des fournitures et du matériel scolaires. Nous luttons contre la déscolarisation massive des enfants. Pour cela, nous sensibilisons les parents et les professeurs sur leurs rôles dans la réussite des enfants à l’école. 
</p><br>
<p>
<strong>Mes passe-temps :</strong><br>


    J’aime bien écrire pour me divertir et surtout pour faire passer certaines frustrations que je ne partage avec personne. 
    J’adore aller au cinéma sauf quand c’est moi qui paye. 
    Je fais beaucoup de sport parce que ça me détend et me permet de retrouver ma sérénité. 
    </p><br>

            <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
        </b-card>


<b-card bg-variant="light"
                text-variant="black">
            <blockquote class="card-blockquote">
                <p>
                   Mes dernières activités associatives et curiosité!
                </p>
                <footer>
                    <small>Someone famous in <cite title="Source Title">Source Title</cite></small>
                </footer>
            </blockquote>
        </b-card>
    <b-card-group columns>
        <b-card title="Campagne de dons de Barinta"
                :img-src="imageBarinta"
                img-fluid
                img-alt="image"
                img-top>
            <p class="card-text">
                Je suis la Vice-présidente de l'association Barinta.<br>
                Cette association a pour objectif de venir en aide des établissements démunis en Afrique de l'Ouest( Mali, Sénégal).
                <router-link to="/projects/barinta"> <b-button variant="primary">En savoir plus</b-button> </router-link>
            </p>
        </b-card>
        <b-card header="Ma vie amoureuse">
            <blockquote class="blockquote mb-0">
                <p>
                <img src="../assets/coeur1.png" width="40px" alt="Nouveau !" />
                </p>
                <p> Hummm, très intéressante, d'ailleurs j'écris des choses là-dessus, alors reveniens plus tard et tu sauras!!! :-)</p>
                <footer class="blockquote-footer">L'amour est à la fois le paradis et l'enfer: Eh oui c'est bien là sa magie et son mystère <br> <cite title="Source Title">Oumou Sow</cite></footer>
            </blockquote>
        </b-card>
        <b-card title="Campagne de communication du forum Find Africa"
                :img-src="imageFind"
                img-fluid
                img-alt="image"
                img-top>
            <p class="card-text">
Le Find Africa est un forum annuel que je coordonne pour l'association CRD depuis 2016. On y aborde de questions essentielles sur l'entreprenariat de la jeunesse africaine, le développe et la paix en Afrique. 
Il est annimé chaque année par de brillants conférenciers.</p>
            <small class="text-muted">Last updated 3 mins ago</small>
        </b-card>
        
       <!--
        <b-card img-src="https://picsum.photos/400/400/?image=41"
                img-fluid
                img-alt="image"
                overlay>
        </b-card>
         -->
        <b-card :img-src="famille"
                img-fluid
                img-alt="image"
                img-top>
            <p class="card-text">
                J'ai la chance d'appartenir à une incroyable et merveilleuse famille nombreuse. En effet,j'ai deux petits frères jumeaux et deux petites soeurs. <br>
                Alors bien-sûre parfois j'ai besoin de calme, ou d'être toute simplement seule juste un instant, mais je me suis
                rendue compte que toute la beauté et la richesse de ma famille se trouve là. On ne se sent jamais seul chez moi, on se sent toujours fort et des solutions à tous les problèmes.
            </p>
            <div slot="footer">
                <small class="text-muted">Ma merveilleuse famille</small>
            </div>
        </b-card>
      
    </b-card-group>
</div>

  </div>
  </div>
</template>

<script>
import imageBarinta from '../assets/imageBarinta.jpeg';
import imageFind from '../assets/imageFind.jpeg';
import famille from '../assets/famille.jpg';

export default {
  name:'about',
  data () {
    return {
      imageBarinta:imageBarinta,
      imageFind: imageFind,
      famille:famille,
    
    }
  }
}
</script>

<style>
.about
{
    background-color: white;
    padding: 30px;
    width: 100%;
   
}

</style>
