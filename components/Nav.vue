<template>
<div class="bar" id="bar">
  <b-navbar type="light" variant="white" toggleable >
    <b-navbar-toggle target="nav_dropdown_collapse"></b-navbar-toggle>
    <b-collapse is-nav id="nav_dropdown_collapse">
      <b-navbar-nav>
      <b-nav-item><router-link to="/">Oumou Sow</router-link></b-nav-item>
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
      &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
      &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
      &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
      &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
      &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;
      &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;

      <b-nav-item><router-link to="/accueil">Accueil</router-link></b-nav-item>
      <b-nav-item><router-link to="/about">À Propos</router-link></b-nav-item>
      <b-nav-item><router-link to="/projets">Projets</router-link></b-nav-item>
      <b-nav-item><router-link to="/contact">Contacter</router-link></b-nav-item>
        <!-- Navbar dropdowns -->
        <!--<b-nav-item-dropdown text="Lang" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
          <b-dropdown-item href="#">RU</b-dropdown-item>
          <b-dropdown-item href="#">FA</b-dropdown-item>
        </b-nav-item-dropdown>
        <b-nav-item-dropdown text="User" right>
          <b-dropdown-item href="#">Account</b-dropdown-item>
          <b-dropdown-item href="#">Settings</b-dropdown-item>
        </b-nav-item-dropdown>-->
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>

</template>

<!--<script>
export default {
  name:'Nav'
}
</script>
-->
<style>

</style>