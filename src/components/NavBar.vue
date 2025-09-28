<script setup>
  function mostrarMenu(){
    
    const navbar = document.getElementsByClassName("navbar")[0];
    const menu = navbar.getElementsByClassName("menu")[0];

    if (navbar.classList.contains('mostrar')){
      navbar.classList.remove('mostrar');
      menu.style.display = '';
      return;
    }

    console.log("entro a version movil")
    menu.style.display = 'block';
    navbar.classList.add('mostrar');

  }
</script>

<template>
  <div class="navbar">
    <div class="marca">
      <button id="btn-menu" @click="mostrarMenu">
        <i class="bi bi-list"></i>
      </button>
      <img id="logo" src="/src/images/deux-logo.png"/>
    </div>
    <ul class="menu">
      <li><a href="#servicios">Servicios</a></li>
      <li><a href="#proyectos">Proyectos</a></li>
      <li><a href="#cursos">Cursos</a></li>
      <li><a href="#contacto">Contacto</a></li>
    </ul>
  </div>
</template>

<style scoped>

  @media only screen and (min-width: 600px){
    #btn-menu{
      display: none;
    }

    .navbar .menu{
      display: flex !important;
    }
  }

  @media only screen and (max-width: 600px) {

    #btn-menu{
      display: block;
      height: 50px;
      width: 50px;
      background: none;
      border: none;
    }

    #btn-menu i{
      color: #000000;
      font-size: 2.5rem;
    }

    .navbar{
      height: auto;
      align-items: center;
      flex-direction: row;
      justify-content: normal !important;
      gap: 50px;
    }

    .navbar .menu{
      display: none;
      width: 100%;
    }

    .mostrar{
      flex-direction: column;
      gap: 10px;
    }

  }

  .marca{
    display: flex;
    align-items: center;
    gap: 20px;
    width: 100%;
  }

  .navbar {
    background: #FFFFFF;
    position: relative;
    display: flex;
    justify-content: space-between;
    padding: 5px;
  }

  .navbar .menu{
    color: black;
    list-style: none;
    align-items: center;
    font-family: 'Roboto Condensed';
    font-size: 1.3rem;
    letter-spacing: 2px;
  }

  .navbar .menu li{
    margin-right: 50px;
  }

  .navbar .menu li > a{
    color: inherit;
    text-decoration: none;
  }

  .navbar #logo{
    height: 45px;
    padding: 2px;
  }
</style>
