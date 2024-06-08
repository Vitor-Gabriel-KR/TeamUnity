<script setup lang="ts">
import BemVindo from './assets/mdlogin/BemVindo.vue';
import CriarEmpresa from  './assets/mdlogin/CriarEmpresa.vue';
import CriarConta from './assets/mdlogin/CriarConta.vue';
import CadastrarEmpresa from './assets/mdlogin/CadastrarEmpresa.vue';


import { ref } from 'vue';
const mostrarPrimeiros = ref(true);
const inverterMostrarPrimeiros = () => {
  mostrarPrimeiros.value = !mostrarPrimeiros.value;
};



</script>

<template>
  <div class="espaco">
  <header v-if="!mostrarPrimeiros">
    <div class="wrapper">
      <CriarEmpresa msg2="Criar empresa" />
    </div>
  </header>

  <main v-if="!mostrarPrimeiros">
    <CadastrarEmpresa />
    <button class="custom-button2" @click="inverterMostrarPrimeiros">VOLTAR</button>
  </main>
</div>

<div class="espaco">
  <header v-if="mostrarPrimeiros">
    <div class="wrapper">
      <BemVindo msg="Bem vindo" />
    </div>
  </header>
    <div>
  <main v-if="mostrarPrimeiros">
    <CriarConta />
    <button class="custom-button" @click="inverterMostrarPrimeiros">CADASTRAR</button>
  </main>
  </div>
</div>
  
</template>

<style>
body{
  margin: 0;
  padding: 0;
  background: linear-gradient(to right, #293C6C 45%, #ffffff 25%, #ffffff 75%);
}
</style>


<style scoped>

.espaco {
  display: flex;
  justify-content: space-between;
}

.side-by-side {
  display: flex;
  flex-direction: column;
}
.custom-button {
  background-color: #293C6C;
  border: 2px solid #293C6C; 
  border-radius: 20px; 
  color: #ffffff; 
  padding: 10px 20px; 
  font-weight: bold;
  font-size: 1.6rem;
  text-transform: uppercase; 
  cursor: pointer; 
  transition: background-color 0.3s, color 0.3s; 
  position: relative;
  margin: 50px; 
  margin-left: auto; 
  margin-right: auto; 
  left: 37%;
}

.custom-button:hover {
  background-color: #ffffff; 
  color: #000000; 
}

.custom-button:active {
  transform: scale(0.95);
}

.custom-button2 {
  background-color: #293C6C;
  border: 2px solid #293C6C; 
  border-radius: 20px; 
  color: #ffffff; 
  padding: 10px 20px; 
  font-weight: bold;
  font-size: 1.6rem;
  text-transform: uppercase; 
  cursor: pointer; 
  transition: background-color 0.3s, color 0.3s; 
  position: relative;
  margin-top: 120px; 
  margin-left: auto; 
  margin-right: auto; 
  left: 41%;
}

.custom-button2:hover {
  background-color: #ffffff; 
  color: #000000; 
}

.custom-button2:active {
  transform: scale(0.95);
}
@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
