<template>
<div class="corpo">
  <div class="texto">
    <h1 class="t1">Bem Vindo ao </h1>
    <h2 class="t2">TeamUnity</h2>
  </div>
  <div class="square">
    <img src="C:\TeamUnity\pages\assets\fotos\pexels-tranmautritam-326502.jpg" alt="Imagem">
  </div>
</div>
</template>

<script setup lang="ts">

</script>

<style scoped>
body {
  margin: 0;
  padding: 0;
  background: linear-gradient(to right, #293C6C 25%, #ffffff 25%, #ffffff 75%);
}
.corpo{
position: absolute;
top: 0px;
align-content: center;
}
.square {
  position: absolute;
  width: 413px;
  height: 423px;
  overflow: hidden;
  margin-left: 8%;
  margin-top: 7%;
  top: 50px;
}
.texto {
  margin-left: 135%;
  margin-top: 40%;
  width: 450px;
  height: 100px;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

</style>


<style scoped >


.t1 {
  font-size: 65px;
  font-weight: bolder;
  color: #313131;
  text-align: center;
  margin: 0;
  padding: 10px;
  
}

.t2 {
  font-size: 100px;
  font-weight: bold;
  color: #000000;
  text-align: center;
  margin: 0;
  padding: 10px;
  letter-spacing: 2px;


}

.square {
  width: 413px;
  height: 423px;
  overflow: hidden;
  margin-left: 8%;
  margin-top: 7%;
  border-radius: 20px;
}


.square img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>
