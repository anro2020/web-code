<template>
  <div class="navbar">
    <img id="logo" src="/src/images/deux-logo.png"/>
    <ul class="menu">
      <li><a href="#servicios">Servicios</a></li>
      <li><a href="#proyectos">Proyectos</a></li>
      <li><a href="#cursos">Cursos</a></li>
      <li><a href="#contacto">Contacto</a></li>
    </ul>
  </div>
</template>

<style scoped>
  .navbar {
    background: #FFFFFF;
    position: relative;
    display: flex;
    justify-content: space-between;
    padding: 5px;
  }

  .navbar .menu{
    color: black;
    display: inline-flex;
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
