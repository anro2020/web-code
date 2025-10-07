<script setup>

import NavBar from './components/NavBar.vue'
</script>

<template>
  <main>
    <NavBar />
    <div class="container">
      <section id="presentacion">
        <div id="descripcion">
          <p>
            Diseño digital, formación tecnológica y soluciones creativas para entornos modernos.
          </p>
          <p>
            Enfoque moderno e innovador para atender las necesidades actuales de comunicación visual y desarrollo digital.
          </p>
        </div>
        <div id="imagen">
          <img src="/src/images/principal.jpg" alt="imagen de bienvenida">
        </div>
      </section>

      <section id="servicios">
        <div id="informacion-servicios">
          <h2>Servicios</h2>
          <div class="elementos">
            <img src="/src/images/magnet-me.jpg"/>
            <div>
              <p class="titulo">Desarrollo de  paginas web</p>
              <div class="descripcion">
                Desarrollo de sitios web modernos, intuitivos y fáciles de navegar, pensados para presentar información de manera clara y atractiva.
              </div>
            </div>
          </div>
          <div class="elementos">
            <img src="/src/images/diagramas.jpg"/>
            <div>
              <p class="titulo">Consultoria y creación de diseños para aplicaciónes web y movíles</p>
              <div class="descripcion">
                Diseño de interfaces para aplicaciones web y móviles, con enfoque en la experiencia del usuario y el crecimiento del negocio.
              </div>
            </div>
          </div>
          <div class="elementos">
            <img src="/src/images/capacitacion.jpeg"/>
            <div>
              <p class="titulo">Capacitación en habilidades digitales</p>
              <div class="descripcion">
                Formación práctica en el uso de computadoras, dispositivos móviles y fundamentos de programación, orientada al desarrollo de habilidades digitales esenciales.
              </div>
            </div>
          </div>
          <div class="elementos">
            <img src="/src/images/disenio.jpg"/>
            <div>
              <p class="titulo">Servicio de diseño grafico</p>
              <div class="descripcion">
                Soluciones visuales alineadas con la identidad del proyecto, enfocadas en comunicar con claridad y generar impacto.
              </div>
            </div>
          </div>
        </div>
      </section>

      <section id="proyectos">
        <div id="informacion-proyectos">
          <h2>Proyectos</h2>
          <div class="elementos">
            <img src="/src/images/magnet-me.jpg"/>
            <div class="descripcion">
              Gimnasio
            </div>
          </div>
          <div class="elementos">
            <img src="/src/images/magnet-me.jpg"/>
            <div class="descripcion">
              Gimnasio
            </div>
          </div>
          <div class="elementos">
            <img src="/src/images/magnet-me.jpg"/>
            <div class="descripcion">
              Ferreteria
            </div>
          </div>
           <div class="elementos">
            <img src="/src/images/magnet-me.jpg"/>
            <div class="descripcion">
              Clinica
            </div>
          </div>
        </div>
      </section>

      <section id="cursos">
        <div id="informacion-cursos">
           <h2>Cursos</h2>
           <div class="elementos">
            <img src="/src/images/magnet-me.jpg"/>
            <div class="descripcion">
              Herramientas digitales al alcance de todos
            </div>
          </div>
           <div class="elementos">
            <img src="/src/images/magnet-me.jpg"/>
            <div class="descripcion">
              Informática Básica para Principiantes
            </div>
          </div>
        </div>
      </section>

      <section id="contacto">
        <div id="informacion-contacto">
          <h2>Contacto</h2>
          <div class="elementos">
           <div id="telefono">
             <i class="bi bi-telephone"></i>
            <span>83-33-19-71-05</span>
           </div>
          </div>
          <div class="elementos">
            <div id="correo">
              <i class="bi bi-envelope"></i>
              <span>deuxsoftware.contacto@gmail.com</span>
            </div>
          </div>
          <div class="elementos">
            <div id="social">
              <i class="bi bi-facebook"></i>
              <span>Deux Software</span>
           </div>
          </div>
        </div>
      </section>
    </div>

    <footer>
      Copyright © 2025 Deux Software
    </footer>
  </main>
</template>

<style scoped>

 @media only screen and (max-width: 600px) {

  .container {
    display: flex !important;
    flex-direction: column !important;
  }

    #presentacion{
      flex-direction: column;
      height: auto !important;
    }

    #presentacion #descripcion{
      width: 100% !important;
      padding: 10px !important;
    }

    #presentacion #descripcion p:nth-of-type(1){
      font-size: 1.5rem !important;
      line-height: 2.3rem !important;
    }

    #presentacion #descripcion p:nth-of-type(2){
      font-size: 1rem !important;
      line-height: 2rem !important;
    }

    #presentacion #imagen {
      width: 100% !important;
    }

    #servicios .elementos{
      flex-direction: column;
      height: auto !important;
    }

    #servicios .elementos .descripcion{
      font-size: 1rem !important;
    }

    #servicios .elementos .titulo{
      font-size: 1.2rem !important;
    }

    #contacto #informacion-contacto .elementos{
      font-size: 1.4rem !important;
      width: 100%;
    }

    #contacto #informacion-contacto .elementos:nth-child(3):before,
    #contacto #informacion-contacto .elementos:nth-child(4):before{
      display: none;
    }
  }

body{
  background-color: #FDFDF5;
}

footer{
  background-color: #2E312A;
  padding: 10px;
  font-family: 'Roboto';
  font-size: 1rem;
  text-align: center;
  color: #F0F2E7;
  letter-spacing: 2px;
}

.container{
    display: block;
    width: 100%;
}

#presentacion {
  background-color: #fdfdf5;
  width: 100%;
  height: 350px;
  display: flex;
}

#presentacion #descripcion{
  width: 60%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 25px;
  padding: 40px;
}

#presentacion #descripcion p:nth-of-type(1){
  color: #000000;
  font-size: 2.35rem;
  font-family: 'Roboto Condensed';
  line-height: 3rem;
  letter-spacing: 2px;
  font-weight: 600;
}

#presentacion #descripcion p:nth-of-type(2){
  color: #000000;
  font-size: 1.6rem;
  font-family: 'Roboto Condensed';
  line-height: 2.5rem;
  letter-spacing: 2px;
  font-weight: 100;
}

#presentacion #imagen{
  width: 40%;
  display: flex;
  background-color: blueviolet;
}

#presentacion #imagen img{
  width: 100%;
}

#servicios{
  background-color: #3F4A35;
}

#informacion-servicios{
  padding: 30px;
  display: flex;
  justify-content: center;
}

#servicios #informacion-servicios{
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
}

#servicios h2{
  text-align: center;
  color: #FFFFFF;
  font-family: 'Roboto Condensed';
  font-size: 2.1rem;
  letter-spacing: 2px;
  width: 100%;
}

#servicios .elementos{
  background-color: #E9E9E9;
  display: flex;
  width: 700px;
  height: 230px;
}

#servicios .elementos .titulo{
  font-family: 'Roboto Condensed';
  font-size: 1.3rem;
  color: #000000;
  padding: 10px;
  height: 30%;
  line-height: 2rem;
  letter-spacing: 1.1px;
  align-content: center;
}

#servicios .elementos .descripcion{
  font-family: 'Roboto Condensed';
  font-size: 1.2rem;
  color: #676767;
  padding: 10px;
  letter-spacing: 1.1px;
  line-height: 2rem;
  display: flex;
  flex-direction: column;
}

#servicios .elementos img{
  width: 330px;
}

#proyectos{
  background-color: #DAE7CA;
}

#proyectos #informacion-proyectos{
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
  justify-content: center;
  padding: 30px;
}

#proyectos #informacion-proyectos > .elementos{
  background: white;
  width: 330px;
  border-radius: 5px;
  display: flex;
  flex-direction: column;
}

#proyectos .descripcion {
  font-family: 'Roboto Condensed';
  font-size: 1.3rem;
  color: #000000;
  letter-spacing: 1px;
  padding: 10px;
}

#proyectos #informacion-proyectos img{
  width: 100%;
}

#proyectos h2{
   color: #000000;
   text-align: center;
   font-family: 'Roboto Condensed';
   font-size: 2.1rem;
   letter-spacing: 2px;
   width: 100%;
}

#cursos{
  background-color: #F0F2E7;
}

#cursos h2{
   color: #000000;
   text-align: center;
   font-family: 'Roboto Condensed';
   font-size: 2.1rem;
   letter-spacing: 2px;
   width: 100%;
}

#cursos #informacion-cursos{
  padding: 30px;
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: center;
}

#cursos #informacion-cursos > .elementos{
    background: white;
    width: 330px;
    border-radius: 5px;
    display: flex;
    flex-direction: column;
}

#cursos .descripcion {
  font-family: 'Roboto Condensed';
  font-size: 1.3rem;
  color: #000000;
  letter-spacing: 1px;
  padding: 10px;
}

#cursos #informacion-cursos img{
  width: 100%;
}

#contacto{
  background-color: white;
}

#contacto h2{
  color: #000000;
  text-align: center;
  font-family: 'Roboto Condensed';
  font-size: 2.1rem;
  letter-spacing: 2px;
  width: 100%;
}

#contacto #informacion-contacto{
  padding: 30px;
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: center;
  background-color: #FDFDF5;
}

#contacto #informacion-contacto .elementos{
  font-size: 1.7rem;
  color: #747474;
  display: flex;
}

#contacto #informacion-contacto .elementos > #telefono{
  gap: 15px;
  display: flex;
  align-items: center;
}

#contacto #informacion-contacto .elementos > #correo{
  gap: 15px;
  display: flex;
  align-items: center;
}

#contacto #informacion-contacto .elementos > #social{
  gap: 15px;
  display: flex;
  align-items: center;
}

#contacto #informacion-contacto .elementos:nth-child(3):before,
#contacto #informacion-contacto .elementos:nth-child(4):before{
    content: '';
    border-left: 3px solid #747474;
    width: 20px;
    height: 40px;
}

</style>
