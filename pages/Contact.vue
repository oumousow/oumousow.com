<template>
<div id="contacter" class="contacter">
<Form></Form>
<div id="contenu" class="contenu">

<a href="https://www.facebook.com/adjaoumousow" title="Facebook" class="facebook_ico soc_circle" target="_blank" style="width: 65px; height: 65px; font-size: 16px;line-height:70px;"><span><img src="https://img.icons8.com/color/104/000000/facebook.png"></span></a>
<a href="https://www.linkedin.com/in/adja-s-b02787a9?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BSzfsSP5fRpSSs7GzP7so%2Fw%3D%3D" title="linkedin" class="linkedin" target="_blank" style="width: 65px; height: 65px; font-size: 16px;line-height:70px;"><span><img src="https://img.icons8.com/color/104/000000/linkedin.png"></span></a>

</div>
</div>
</template>

<script>
import Form from '@/components/Form'
import image1 from '@/components/Form'
export default 
{  
  name: 'contact',
  components: 
{
Form,

  }
}

</script>

<style>
.contacter
{
     background:url("../assets/image1.png") no-repeat center fixed;
    margin:0px;
    padding: 380px;
  -webkit-background-size: cover; /* pour Chrome et Safari */
  -moz-background-size: cover; /* pour Firefox */
  -o-background-size: cover; /* pour Opera */
  background-size: cover; /* version standardisée */
  background-position:100% 0%;
}
.contenu
{
margin:0px;
padding:0px;
background-color: rgba(0, 0, 0, 0.0);
background-position: 0% 0%;
}
</style>
