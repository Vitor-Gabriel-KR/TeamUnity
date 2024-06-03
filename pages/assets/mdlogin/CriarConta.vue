<template>
  <div class="espaco">
    <div>
      <h1 id="titulo">Criar conta</h1>
    </div>
    <div id="container">
      <input type="text" id="texto" placeholder="Nome">
      <input type="text" id="texto" placeholder="Email">
      <input type="password" id="texto" placeholder="Senha">
    </div>
  </div>
</template>

<script>



</script>

<style scoped>
.espaco {
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 300px;
  width: 800px;
  margin-top: 50px; 
}

#titulo {
  font-size: 50px;
  color: #293C6C; 
  text-align: center;
  font-family: 'PoetsenOne', sans-serif;
  font-weight: 800;
}

#container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

input {
  font-size: medium;
  height: 50px;
  width: 450px; 
  margin-bottom: 10px;
  background-color: #D9D9D9;
  color: #929292;
  border-radius: 5px;
  outline: none;
  padding-left: 50px; 
}


</style>