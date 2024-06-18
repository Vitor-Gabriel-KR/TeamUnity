<template>
  <div>
    <header class="header">
      <div class="left-icon">
        <i class="fas fa-bars">TeamUnity</i>
      </div>
      <p class="header-text"></p>
      <div class="right-icon">
        <i class="fas fa-user"></i>
      </div>
    </header>
    <div class="content">
      <!-- Conteúdo principal da página vai aqui -->
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderComponent'
}
</script>

<style scoped>

.header {
  background-color: #2A2E34;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: white;
  position: fixed; 
  top: 0;
  right: 0; 
  width: 100%;
  height: 40px;
  z-index: 1000; /* Certifique-se que o header esteja acima dos outros elementos */
}

.left-icon, .right-icon {
  display: flex;
  margin-left: 22px;
  align-items: left;
}

.header-text {
  margin: 0;
  font-size: 16px;
}

.content {
  padding-top: 40px; /* Ajuste o padding-top para corresponder à altura do header */
}
</style>