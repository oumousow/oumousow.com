<template>
<div class="astuces">
<div id="contacter" class="contacter">

<div class="form">
<Form></Form>
</div>
<div id="contenu" class="contenu">
<a href="https://www.facebook.com/adjaoumousow" title="Facebook" class="facebook_ico soc_circle" target="_blank" style="width: 45px; height: 45px; font-size: 6px;line-height:50px;"><span><img src="https://img.icons8.com/color/74/000000/facebook.png"></span></a>
<a href="https://www.linkedin.com/in/adja-s-b02787a9?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BSzfsSP5fRpSSs7GzP7so%2Fw%3D%3D" title="linkedin" class="linkedin" target="_blank" style="width: 45px; height: 45px; font-size: 6px;line-height:50px;"><span><img src="https://img.icons8.com/color/74/000000/linkedin.png"></span></a>
</div>
</div>
</div>
</template>

<script>
import Form from '@/components/Form'
export default 
{  
  name: 'contact',
  components: 
{
Form,

  }
}

</script>
<!--
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
}
.form
{
padding-left: 5px;
padding-right: 5px;

margin-top: 10px;
background-color: rgba(0, 0, 0, 0.1); 
}

</style>
-->
<style>
.astuces
{
    background-color: white;

}
.contacter
{
  padding: 40px;
}
.contenu
{
  padding-left: 600px;
  padding-top: 100px;

}
</style>
