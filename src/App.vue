<script setup>
</script>

<template>

</template>

<style>
/* Reset básico */
body {
  /* background-color: white; */
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  padding-top: 100px;
}

/* Estilos del navbar */
nav {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 30px;
  background-color: white;
  color: black;
  position: fixed;
  border-bottom: 1px solid black;
  top: 0;
  left: 0;
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


}

.contenedor {
  min-height: 300px;
  position: fixed;
  top: 90px;
  left: 5px;
  margin-left: 100px;

  width: 100%;
  margin-bottom: 50px;
}

.titulo {
  position: absolute;
  color: black;
  background-color: rgba(255, 0, 0, 0.258);
  font-size: 11vh;
  font-family: Arial, sans-serif;
  font-stretch: expanded;
  font-weight: bold;
  z-index: 20;
  width: 100%;
}

.capa_logo {
  position: absolute;
  z-index: 10;
  /* opacity: 0; */
  
  /* animation: apareceLogo 5s forwards; */
}

.capa_logo img {
  position: fixed;
  width: 840px;
  top: 190px;
  left: -90px;
}


.t_1 {
  animation: apareceTitulo 2s cubic-bezier(0.25, 0.1, 0.25, 1);
  /* z-index: 20; */

}

.t_2 {
  animation: apareceTitulo 2s cubic-bezier(0.4, 0.1, 0.25, 1);
  /* z-index: 20; */

}




@keyframes apareceTitulo {
  0% {
    transform: translateX(-100%);
  }

  100% {
    transform: translateX(0);
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

