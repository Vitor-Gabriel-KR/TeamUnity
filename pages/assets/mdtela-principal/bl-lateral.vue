<template>
  <div>
    <div class="barra-lateral">
      <div class="perfil">
        <div class="foto-perfil">
          <img src="/imagens/admin.jpg" alt="Foto do Perfil" />
        </div>
        <div class="info-perfil">
          <p class="nome-perfil">Vitor </p>
          <p class="cargo-perfil">Admin</p>
        </div>
      </div>
      <p class="linha"></p>
      <p class="titulo-secao">Seus quadros</p>
  
      <div class="secao-interativa">
        <div class="item-interativo">
          Funcionários
        </div>
      </div>
      
      <p class="titulo-secao">Cadastros</p>
      <div class="secao-interativa">
        <div class="item-interativo" >
          <a class ="a" href="http://127.0.0.1:8000/funcionario/?format=api">Funcionários</a>
      </div>
      </div>

      <div class="status-container">
    <h2 class="status-title">Status</h2>
    <ul class="status-list">
      <li class="status-item">
        <span class="service-name">API:</span>
        <span class="status-online">Online</span>
      </li>
      <li class="status-item">
        <span class="service-name">Cadastro:</span>
        <span class="status-online">Online</span>
      </li>
    </ul>
  </div>
    </div>
    <div class="segundo-header">
      <p class="nome-empresa">Iluminaty Comporations - empresa com foco na dominação global </p>
    </div>
    <div class="caixab">
    </div>
  </div>
</template>

<style scoped>
.status-container {
  background-color: #b9b9b9;
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 20px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  max-width: 300px;
  margin: auto;
}

.status-title {
  font-size: 24px;
  font-weight: bold;
  color: #333;
  margin-bottom: 15px;
  text-align: center;
}

.status-list {
  list-style: none;
  padding: 0;
}

.status-item {
  display: flex;
  justify-content: space-between;
  padding: 10px 0;
  border-bottom: 1px solid #eee;
}

.status-item:last-child {
  border-bottom: none;
}

.service-name {
  font-size: 18px;
  color: #555;
}

.status-online {
  font-size: 18px;
  font-weight: bold;
  color: green;
}
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
  z-index: 1000; 
}

.left-icon, .right-icon {
  display: flex;
  align-items: center;
}

.header-text {
  margin: 0;
  font-size: 1rem;
}
.linha{
  height: 1px;
  width: 150px;
  background-color:  #727272;
}
.barra-lateral {
  width: 210px;
  height: calc(100vh - 40px); 
  background-color: #D5D5D5;
  padding: 10px;
  display: flex;
  flex-direction: column;
  align-items: center;
  position: fixed;
  left: 0;
  top: 40px;
  z-index: 999; 
  overflow-y: auto; 
}

.perfil {
  display: flex;
  align-items: center;
  margin-top: 10px;
  margin-bottom: 20px;
  margin-left: 10px;
  align-self: flex-start;
  
}

.foto-perfil {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  overflow: hidden;
  margin-right: 10px;
  background-color: #9bb0ca;
  border: 2px solid #727272;
}

.foto-perfil img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.info-perfil {
  display: flex;
  flex-direction: column;
}

.nome-perfil {
  font-size: 28px;
  color: black;
  margin: 0;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.cargo-perfil {
  font-size: 16px;
  color: #969595;
  margin: 0;
}

.titulo-secao {
  font-size: 21px;
  color: black;
  margin-top: 20px;
  margin-bottom: 20px;
  margin-right: 70px;
  margin-left: 20px;
}

.secao-interativa {
  width: 80%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin-left:20px;
  
}

.item-interativo {
  width: 100%;
  padding: 5px 10px;
  margin: 5px 0;
  background: rgb(177, 177, 177) ;
  color: black;
  cursor: pointer;
  text-align: left;
  border-radius: 5px;
  font-size: 18px;
}
.a{
  text-decoration: none;
}
.item-interativo:hover {
  background-color: #727272;
}
.item-interativo2:hover {
  background: #727272 ;
}

.segundo-header {
  width: calc(100% - 210px); 
  height: 65px;
  background: rgb(2,0,36);
  background: radial-gradient(circle, rgba(2,0,36,1) 15%, rgba(255,139,0,1) 26%, rgba(9,9,121,1) 51%);
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 35px;
  box-sizing: border-box;
  position: fixed;
  top: 40px;
  right: 0;
  z-index: 998; /* Certifique-se de que o segundo header esteja acima do conteúdo principal */
}

.nome-empresa {
  font-size: 24px;
  color: white;
  margin: 0;
}

.barra-pesquisa-container {
  display: flex;
  align-items: center;
}

.barra-pesquisa {
  width: 200px;
  height: 25px;
  padding: 5px;
  border-radius: 5px 0 0 5px;
  border: none;
  box-sizing: border-box;
}

.botao-filtro {
  height: 35px;
  padding: 0 10px;
  border-radius: 0 5px 5px 0;
  border: none;
  background-color: white;
  color: #293C6C;
  cursor: pointer;
  box-sizing: border-box;
}

.caixab {
  margin-top: 37px; 
  margin-left: 210px;
  padding: 10px;
}
</style>