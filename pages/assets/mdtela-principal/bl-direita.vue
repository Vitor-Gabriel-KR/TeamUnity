<template>
    <div class="sidebar">
      <div class="funcao">
        <h2 class="cargo">Gerente - 1</h2>
        <div class="funcionarios">
          <img src="" alt="photo" class="photo" >
          <p class="status"></p>
        </img>
          <div class="textos">
            <p class="nome1">Nome </p>
          </div>
        </div>
      </div>

      <div class="funcao">
        <h2 class="cargo">TeamLeaders - 4</h2>
        <div class="funcionarios">
          <img src="" alt="photo" class="photo" >
          <p class="status"></p>
        </img>
          <div class="textos">
            <p class="nome1">Nome </p>
          </div>
        </div>
        <div class="funcionarios">
          <img src="" alt="photo" class="photo" >
          <p class="status"></p>
        </img>
          <div class="textos">
            <p class="nome1">Nome </p>
          </div>
        </div>
        <div class="funcionarios">
          <img src="" alt="photo" class="photo" >
          <p class="status"></p>
        </img>
          <div class="textos">
            <p class="nome1">Nome </p>
          </div>
        </div>
        <div class="funcionarios">
          <img src="" alt="photo" class="photo" >
          <p class="status"></p>
        </img>
          <div class="textos">
            <p class="nome1">Nome </p>
          </div>
        </div>
      </div>

    </div>
  </template>
  
  <style scoped>
  .sidebar {
  width: 300px;
  height: 1350px;
  background-color: #d0cfff;
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
}
.status {
  height: 11px;
  width: 11px;
  background-color: #33FB3B;
  border-radius: 50%;
  position: absolute;
  margin-left: 48px;
  margin-top: 59px;
}
.funcao {
  margin-top: 15px;
  margin-left: 25px;
}
.funcionarios {
  display: flex;
  align-items: center;
}
.photo {
  height: 45px;
  width: 45px;
  margin-right: 12px;
  margin-left: 13px;
  margin-top: 12px;
  background-color: #6D7993;
  border-radius: 50%;
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
  