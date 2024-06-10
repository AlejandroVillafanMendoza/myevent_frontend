<template>
  <div class="hero-container">
    <div class="hero-image">
      <div class="hero-text">
        <br><br><br><br><br><br><br>
        <br>
        <button id="nuestras_ofertas" @click="gotoNuestras" class="ofertas_boton">Productos y Servicios</button>
      </div>
    </div>
  </div>
</template>

<script setup>
const gotoNuestras = () => {
  window.location.href = '/products'; 
}
</script>

<style scoped>
.hero-container {
  position: relative;
  height: 100vh;
  overflow: hidden;
}

.hero-image {
  background-image: url('/public/img/hero_myevent.png');
  height: 100%;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}

.hero-text {
  text-align: center;
  font-family: initial;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: #f8ffc0;
  text-shadow: 
    -2px -2px 0 #ffc0cb,  
     2px -2px 0 #ffc0cb,
    -2px  2px 0 #ffc0cb,
     2px  2px 0 #ffc0cb; 
}

.hero-text button {
  font-family: initial;
  border: none;
  outline: 0;
  display: inline-block;
  padding: 10px 25px;
  color: rgb(255, 255, 255);
  background-color: #73f0eb;
  text-align: center;
  cursor: pointer;
  border-radius: 10px;
}

.hero-text button:hover {
  background-color: #ffffff9e;
  color: rgb(2, 1, 1);
  transform: scale(1.15);
}

.ofertas_boton {
  margin-left: 15px;
  margin-top: 200px;
  height: 100px;
  font-size: 25px;
}
</style>
