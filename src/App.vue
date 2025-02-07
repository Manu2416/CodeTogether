<script setup>
</script>

<template>
  <header>
    <nav>
      <div class="logo">
        <img src="@/assets/fotos/logo_morado.png" alt="Logo Morado">
        <h2>Innova Studio</h2>
      </div>
      <div class="nav_derecha">
        <a href=""> Home </a>
        <a href="">Portafolio</a>
        <a href="">Rest</a>
      </div>
    </nav>
</header>
  
  <main>
    <section class="contenedor">
      <article class="titulo">
        <p class="t_1">Welcome to</p>
        <p class="t_2">Innova.</p>
      </article>

      <article class="capa_logo">

        <img src="@/assets/fotos/logo_morado.png" alt="Logo Morado">
      </article>
   </section>
  </main>

  <!-- <p>Graphic design studio</p>
  <div>Aquí lo que se mueve</div>
  <div>Aquí ellos</div>
  <div>Contactos y branding</div> -->

  <footer>
    © 2035 by Business Name. Built on Wix Studio
  </footer>
</template>

<style>
/* Reset básico */


html, body {
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  height: 100%;
}

body {
  display: flex;
  flex-direction: column;
  height: 100vh;
}
header{
  width: 100%;
}
/* Estilos del navbar */
nav {
  display: flex;
  justify-content: space-between;
  padding: 20px 30px;
  background-color: white;
  color: black;
  border-bottom: 1px solid black;
 
}

/* Logo y nombre */
.logo {
  display: flex;
  align-items: center;
  gap: 10px;
}

.logo img {
  height: 40px;
  object-fit: contain;
}

/* Ícono de menú */
.menu-icon {
  height: 30px;
  cursor: pointer;
}

.nav_derecha {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
  color: white;


}
.nav_derecha:hover{
 color: red;
}
main{
  width: 100%;
  display: flex;
}

.contenedor{
  height: 600px;
  width: 100%;
  display: flex;
  background-color: rgba(0, 0, 255, 0.567);
}
.titulo{
  overflow: hidden;
  display: flex;
  flex-direction: column;
  color: black;
  width: 100%;

  font-family: Arial, sans-serif;
  font-weight: bold;
  z-index: 20;
  padding: 20px;
  
  
}

.t_2{
  border: solid rgb(219, 33, 33) 1px;
  margin-top: -150px;
  font-size: 25vh;
  
}
.t_1{
  margin-top: -1px;
  border: solid rgb(219, 33, 33) 1px;
  font-size: 25vh;
}


.capa_logo {
  position: absolute;
  z-index: 10;
  /* opacity: 0; */
  
  /* animation: apareceLogo 5s forwards; */
}

.capa_logo img {
  width: 840px;
  top: 190px;
  left: -90px;
}
.t_1 {
  animation: apareceTitulo 2s ease forwards;
  /* z-index: 20; */

}

.t_2 {
  animation: apareceTitulo 2.5s ease forwards;
  /* z-index: 20; */

}


footer {
  width: 100%;
  height: 100px;
  background-color: black;
  color: white;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: auto;
}



@keyframes apareceTitulo {
  0% {
    transform: translateX(-100%);
  }

  100% {
    transform: translateX(10%);
  }
}

@keyframes apareceLogo {
  0% {
    left: -100%;
    opacity: 0;
  }

  50% {
    left: 50%;
    opacity: 1;
    transform: translate(-50%, -50%);
  }

  100% {
    left: 100%;
    opacity: 0;
  }


}





/* .titulo img {
  position: absolute;
  z-index: 10;
  top: 20PX;
} */
</style>

