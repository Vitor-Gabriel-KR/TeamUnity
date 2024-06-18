<script setup lang="ts">
import dashcentral from './assets/mdtela-principal/dash-central.vue';
import HeaderComponent from './assets/mdtela-principal/header.vue';
import blesquerda from './assets/mdtela-principal/bl-lateral.vue';
import bldireita from './assets/mdtela-principal/bl-direita.vue';


</script>

<template>
    <HeaderComponent></HeaderComponent>
    <blesquerda></blesquerda>
    <bldireita></bldireita>
    <dashcentral></dashcentral> 
</template>

<style scoped >
body{
    background-color: white;
}

</style>