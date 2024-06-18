<script setup lang="ts">
defineProps<{
  msg2: string
}>()
</script>

<template>
  <div class="greetings">
    <h2 class="green">{{ msg2 }}</h2>
    <h3>
        Crie e configure sua empresa com facilidade 
        Simplifique a gestão de sua equipe
        e otimize processos
    </h3>
    <NuxtLink to="/tela-principal" class="custom-button">Criar</NuxtLink>
    <p >Ou <a href="https://www.example.com">entre</a> em sua empresa.</p>
  </div>
</template>

<style scoped>
a{
  color:rgb(9, 160, 165);
}
p{
  color: #ffffff;
    top: 100%;
  font-size: 1.2rem;
  text-align: center; 
  width: 55%; 
  position: relative; 
  left: 50%; 
  transform: translateX(-50%);
  margin-top: 20px; 
  text-align: center;
}
h2 {
  font-weight:900;
  font-size: 3.5rem;
  position: relative;
  top: 100%;
  color: #ffffff;
  left: 20%;
}
h3 {
  top: 100%;
  color: #ffffff;
  font-size: 1.2rem;
  width: 70%; 
  position: relative; 
  left: 50%; 
  transform: translateX(-50%);
  margin-top: 10px; 
  text-align: center;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}

.custom-button {
  background-color: transparent;
  border: 2px solid #ffffff; 
  border-radius: 20px; 
  color: #ffffff; 
  width: 45%;
  padding: 10px 20px; 
  font-weight: bold;
  font-size: 1.6rem;
  text-transform: uppercase; 
  cursor: pointer; 
  transition: background-color 0.3s, color 0.3s; 
  position: relative;
  top: 100%;
  margin: 0 10px;
  margin: 10px; 
  margin-left: auto; 
  margin-right: auto; 
  left: 37%;
  bottom: 30%;
  text-decoration: none;
  
}

.custom-button:hover {
  background-color: #ffffff; 
  color: #000000; 
}

.custom-button:active {
  transform: scale(0.95);
}
</style>
