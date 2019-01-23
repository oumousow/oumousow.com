<template>
<div>
  <div class="about">
   
     <div>
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
        <b-card header="Quote">
            <blockquote class="blockquote mb-0">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
                <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
            </blockquote>
        </b-card>
        <b-card title="Campagne de communication du forum Find Africa"
                :img-src="imageFind"
                img-fluid
                img-alt="image"
                img-top>
            <p class="card-text">
                This card has supporting text below as a natural lead-in to additional content.
            </p>
            <small class="text-muted">Last updated 3 mins ago</small>
        </b-card>
        <b-card bg-variant="primary"
                text-variant="white">
            <blockquote class="card-blockquote">
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.
                </p>
                <footer>
                    <small>Someone famous in <cite title="Source Title">Source Title</cite></small>
                </footer>
            </blockquote>
        </b-card>
        <b-card title="Title">
            <p class="card-text">
                This card has supporting text below as a natural lead-in to additional content.
            </p>
            <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
        </b-card>
        <b-card img-src="https://picsum.photos/400/400/?image=41"
                img-fluid
                img-alt="image"
                overlay>
        </b-card>
        <b-card img-src="https://picsum.photos/400/200/?image=41"
                img-fluid
                img-alt="image"
                img-top>
            <p class="card-text">
                This is a wider card with supporting text below as a natural lead-in to additional content. This card has even longer content
                than the first.
            </p>
            <div slot="footer">
                <small class="text-muted">Footer Text</small>
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
export default {
  name:'about',
  data () {
    return {
      imageBarinta:imageBarinta,
      imageFind: imageFind,
    }
  }
}
</script>

<style>
.about
{
    background-color: white;
    padding: 20px;
    width: 100%;
   
}
</style>
