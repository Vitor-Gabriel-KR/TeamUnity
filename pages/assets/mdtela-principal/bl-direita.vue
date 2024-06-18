<template>
  <div class="sidebar">
    <div class="funcao">
      <h2 class="cargo">Gerente - 2</h2>
      <div class="funcionarios">
        <img src="/imagens/admin.jpg" alt="photo" class="photo" />
        <p class="status"></p>
        <div class="textos">
          <p class="nome1">Vitor</p>
        </div>
      </div>
      <div class="funcionarios">
        <img src="/imagens/admin.jpg" alt="photo" class="photo" />
        <p class="status2"></p>
        <div class="textos">
          <p class="nome1">Gustavo</p>
        </div>
      </div>
    </div>

    <div class="funcao">
      <h2 class="cargo">TeamLeaders - 4</h2>

      <div class="funcionarios" @click="setId(2)">
        <img src="/imagens/juan.jpeg" alt="photo" class="photo" />
        <p class="status"></p>
        <div class="textos">
          <p class="nome1">Juan</p>
        </div>
      </div>
      <div class="funcionarios" @click="setId(3)">
        <img src="/imagens/DIlma.png" alt="photo" class="photo" />
        <p class="status2"></p>
        <div class="textos">
          <p class="nome1">Dilma Rouseff</p>
        </div>
      </div>
      <div class="funcionarios" @click="setId(4)">
        <img src="/imagens/kratos.png" alt="photo" class="photo" />
        <p class="status2"></p>
        <div class="textos">
          <p class="nome1">Kratos do godi</p>
        </div>
      </div>

      <div class="funcionarios" @click="setId(5)">
        <img src="/imagens/Naruto.png" alt="photo" class="photo" />
        <p class="status"></p>
        <div class="textos">
          <p class="nome1">Naruto Uzumaki</p>
        </div>
      </div>
      
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      id: 4 
    };
  },
  methods: {
    setId(newId) {
      this.id = newId;
    }
  }
};
</script>
<style>
::-webkit-scrollbar {
  width: 15px;
}

::-webkit-scrollbar-track {
  background: #293C6C;
}

::-webkit-scrollbar-thumb {
  background: #eeeeee;
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: #cccccc;
}
</style>

<style scoped>
.sidebar {
  width: 300px;
  height: 1350px;
  background-color: #D5D5D5;
  float: right;
  position: static;
}

.sidebar::-webkit-scrollbar {
  width: 15px;
}
.sidebar::-webkit-scrollbar-track {
  background: #293C6C;
}
.sidebar::-webkit-scrollbar-thumb {
  background: #FFFFFF;
  border-radius: 10px;
}
.sidebar::-webkit-scrollbar-thumb:hover {
  background: #CCCCCC;
}

.nome1 {
  color: rgb(0, 0, 0);
  font-size: 18px;
  font-weight: 500;
  width: 180px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  border-bottom: 1px solid  #727272;
}
.status {
  height: 11px;
  width: 11px;
  background-color: #33FB3B;
  border-radius: 50%;
  position: absolute;
  margin-left: 48px;
  margin-top: 45px;
}
.status2 {
  height: 11px;
  width: 11px;
  background-color: #d80808;
  border-radius: 50%;
  position: absolute;
  margin-left: 48px;
  margin-top: 45px;
}
.funcao {
  margin-top: 15px;
  margin-left: 25px;
}
.funcionarios {
  display: flex;
  align-items: center;
  border: 2px solid  #c5c5c5;
  border-radius: 10px;
  margin-top: 15px;
  cursor: pointer;
}

.photo {
  height: 45px;
  width: 45px;
  margin-right: 12px;
  margin-left: 13px;
  background-color: #6D7993;
  border-radius: 50%;
  border: 2px solid #727272;
}
.cargo {
  color: rgb(0, 0, 0);
  font-size: 20px;
  font-weight: lighter;
  margin-bottom: 10px;
}
.textos {
  color: black;
}
</style>