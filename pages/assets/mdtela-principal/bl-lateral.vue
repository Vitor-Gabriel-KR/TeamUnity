<template>
  <div>
    <div class="barra-lateral">
      <div class="perfil">
        <div class="foto-perfil">
          <img src="" alt="Foto do Perfil" />
        </div>
        <div class="info-perfil">
          <p class="nome-perfil">Nome</p>
          <p class="cargo-perfil">Cargo</p>
        </div>
      </div>
      <p class="titulo-secao">Seus quadros</p>
  
      <div class="secao-interativa">
        <div class="item-interativo">
          Funcionários
        </div>
        <div class="item-interativo2">
          Projetos
        </div>
      </div>
      <p class="titulo-secao">Cadastros</p>
      <div class="secao-interativa">
        <div class="item-interativo">
          Funcionários
        </div>
        <div class="item-interativo2">
          Projetos
        </div>
      </div>
      <div class="secao-gestao">
        <p class="titulo-secao">Gestão De Membros</p>
        <p class="titulo-secao">Gestão De Equipes</p>
        <p class="titulo-secao">Configurações Dos Cards</p>
      </div>
    </div>
    <div class="segundo-header">
      <p class="nome-empresa">Nome da empresa</p>
      <div class="barra-pesquisa-container">
        <input type="text" class="barra-pesquisa" placeholder="Pesquisar" />
        <button class="botao-filtro">Filtro</button>
      </div>
    </div>
    <div class="caixab">
    </div>
  </div>
</template>

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

.barra-lateral {
  width: 210px;
  height: calc(100vh - 40px); 
  background-color: #323535;
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
  color: rgb(255, 255, 255);
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
  font-size: 20px;
  color: rgb(255, 255, 255);
  margin-top: 20px;
  margin-bottom: 20px;
  margin-right: 22px;
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
  background: rgb(165, 138, 223) ;
  color: rgb(255, 255, 255);
  cursor: pointer;
  text-align: left;
  border-radius: 5px;
  font-size: 18px;
}

.item-interativo2 {
  width: 100%;
  padding: 5px 10px;
  margin: 5px 0;
  background-color: #ecce96;
  color: rgb(255, 255, 255);
  cursor: pointer;
  text-align: left;
  border-radius: 5px;
  font-size: 18px;
}

.item-interativo:hover {
  background-color: #ecce96;
}
.item-interativo2:hover {
  background: rgb(165, 138, 223) ;
}

.secao-gestao {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin-top: 65px;
  
}

.secao-gestao .titulo-secao {
  margin-bottom: 1px;
  font-size: 16px;
}

.segundo-header {
  width: calc(100% - 210px); 
  height: 65px;
  background-color: #293C6C;
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