<template>
  <div>
    <div class="cima"></div>
    <div>
      <Transition name="fade">
        <PrimeiroContato v-if="!showSecondScreen"></PrimeiroContato>
      </Transition>
      <Transition name="fade">
        <Explicacao v-if="showSecondScreen"></Explicacao>
      </Transition>
    </div>
    <div class="baixo"></div>
  </div>
</template>

<script setup lang="ts">
import {  onMounted, onBeforeUnmount } from 'vue';
import { Transition } from 'vue';


import PrimeiroContato from './assets/mdtela-inicial/PrimeiroContato.vue';
import Explicacao from './assets/mdtela-inicial/Explicacao.vue';

const showSecondScreen = ref(false);
const scrolled = ref(0);

const toggleScreen = () => {
  showSecondScreen.value = !showSecondScreen.value;
};

const handleScroll = () => {
  scrolled.value = window.scrollY;
  if (scrolled.value > 70 && !showSecondScreen.value) {
    toggleScreen();
  } else if (scrolled.value <= 19 && showSecondScreen.value) {
    toggleScreen();
  }
};

onMounted(() => {
  window.addEventListener('scroll', handleScroll);
});

onBeforeUnmount(() => {
  window.removeEventListener('scroll', handleScroll);
});
</script>

<style scoped>
.cima {
  width: 100%;
  height: 70vh; /* Aumentando a altura para criar uma área de rolagem maior */
  background-color: aquamarine;
  opacity: 0.1;
}

.baixo {
  width: 100%;
  height: 50vh; /* Aumentando a altura para criar uma área de rolagem maior */
  background-color: aquamarine;
  opacity: 0.1;
}

.fade-enter-active, .fade-leave-active {
  transition: opacity 0.5s ease;
}

.fade-enter-from, .fade-leave-to {
  opacity: 0;
}
</style>
