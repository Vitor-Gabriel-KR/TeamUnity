<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <div class="espaco1">
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      para manter-se conectado com 
      a gente efetue o login no nosso sistema
    </h3>
    <button class="custom-button">ENTRAR</button>
  </div>
</div>
</template>

<style scoped>
.espaco1{
  top:25%;
  display: flex;
  position: absolute;
  flex-direction: column;
  align-items: center;
}
h1 {
  font-weight: 900;
  font-size: 3.5rem;
  position: relative;
  top: -40px;
  color: #ffffff;
  left: 25%;
}

h3 {
  top: -40px;
  font-size: 1.2rem;
  text-align: center; 
  width: 55%; 
  position: relative; 
  left: 50%; 
  color: #ffffff;
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
  top: -20px;
  margin: 0 10px;
  margin: 10px; 
  margin-left: auto; 
  margin-right: auto; 
  left: 26%;
  bottom: 30%;
}

.custom-button:hover {
  background-color: #ffffff; 
  color: #000000; 
}

.custom-button:active {
  transform: scale(0.95);
}
</style>