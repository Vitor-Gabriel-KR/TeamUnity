<template>
<div class="corpo2">
  <div class="top">
    <div class="texto2">
      <h1 class="t12">O que é  </h1>
      <h2 class="t22">TeamUnity</h2>
    </div>
    <div class="square2">
    <img src="C:\TeamUnity\pages\assets\fotos\pexels-junior-teixeira-1064069-2047905.jpg" alt="Imagem2">
  </div>
  <div class="container2">
  <p>Team Unity é uma ferramenta web de gestão de funcionários altamente personalizável, projetada para oferecer praticidade e inovação aos gestores. </p>
  <p>Facilita a promoção da coesão da equipe de maneira eficiente.</p>
  <button class="botao">Cadastrar</button>
</div>
</div>
</div>
  </template>
 
 <script setup lang="ts">

 
  </script>


<style >

.corpo2 {
  position: absolute;
  top: 10px;
  align-content: center;
  z-index: 1;
  background: linear-gradient(to bottom left, #091b47 0%, #18274e 50%, #0f265f 75%, #293C6C 100%);
}
.botao{
  
  background-color: rgba(31, 5, 192, 0.8);
  background-color: #293C6C;
  border: 2px solid #ffffff; 
  border-radius: 20px; 
  color: #ffffff; 
  padding: 10px 20px; 
  font-weight: bold;
  font-size: 1.6rem;
  text-transform: uppercase; 
  cursor: pointer; 
  transition: background-color 0.3s, color 0.3s; 
  position: relative;
  margin: 0 10px;
  margin: 20px; 
  margin-left: auto; 
  margin-right: auto; 
  left: 17%;
  bottom: 30%;
}
.botao:hover {
  background-color: #ffffff; 
  color: #000000; 
}

.botao:active {
  transform: scale(0.95);
}
</style>
 <style scoped>
body {
    position: relative;
}
body::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: #1F05C0; 
    opacity: 0.3;
    z-index: -1; 
}

body {
    background: linear-gradient(220deg, #ffffff 1%, #293C6C 50%);
    height: 110vh;
    margin: 0;
    padding: 0;
}
</style>


  <style scoped >

.top{
  margin-top: 500px;
}
.texto2 {
  position: absolute;
  margin-left: 6%;
  margin-top: 4%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}.t12, .t22 {
  font-family: 'Lato', sans-serif;
  color: #ffffff;
  text-align: center;
  margin: 0;
  padding: 10px;
}


.t12 {
  font-size: 80px;
}


.t22 {
  font-size: 90px;
  letter-spacing: 2px;
}


.square2 {
  width: 520px;
  height: 473px;
  border: 2px solid #000;
  background-color: #293C6C;
  overflow: hidden;
  margin-left: 60%;
  margin-top: -10%;
  border-radius:  50px 0 0  50px;
}


.square2 img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.container2 {
    width: 30%;
    margin: 0 auto;
    padding: 20px;
    border-radius: 8px;
    margin-left: 6%;
    margin-top: -17%;
    text-align: left;
  }


  .container2 p {
    font-family: 'Lato', sans-serif;
    font-size: 20px;
    line-height: 1.5;
    color: #ffffff;
  }


  </style>
