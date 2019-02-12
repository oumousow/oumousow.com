<template>
<div class="bar" id="bar">
  <b-navbar 
      class="cowork-nav"
      toggleable="md"
      variant="white" 
      type="light">
      <b-navbar-toggle target="nav_collapse"/>
      
      <b-navbar-brand class="logo" to="/">
        Oumou Sow
      </b-navbar-brand>
      
      <b-collapse 
        id="nav_collapse" 
        is-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-item 
            right
            to="/accueil">Mon Stage</b-nav-item>
          <b-nav-item 
            right
            to="/watcher">Projet Pste</b-nav-item>
          <b-nav-item 
            right
            to="/about">À propos</b-nav-item>
          <b-nav-item 
            right
            to="/projects">Projets</b-nav-item>
          <b-nav-item 
            right
            to="/contact">Contact</b-nav-item>
        </b-navbar-nav>
      </b-collapse>  
    </b-navbar>
  </div>
</template>

<style>
  .bar {
    border-bottom: 1px solid #dddddd;
    margin-bottom: 1rem;
  }
  .bg-container .logo {
    font-weight: 900;
    color: white !important;
    font-size: 1.8rem;
  }
  .logo {
    font-weight: 900;
    color: #333 !important;
    font-size: 1.8rem;
  }
</style>