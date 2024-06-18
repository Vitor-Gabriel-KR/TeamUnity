<template>
  <div>
    <NuxtPage/>
  </div>
</template>

<script>
import './plugins/axios.js'
import axios from 'axios';

axios.get('/funcionario')
.then((response) => {
  response=dadosFuncionario;
})

</script>
