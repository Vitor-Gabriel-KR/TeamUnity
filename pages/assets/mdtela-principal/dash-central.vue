<template>
  <div class="divisor">
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
        


      </div>
    </div>
    
    <div class="container">
      <div class="quadrado">
        <div class="conteudo">
          <img src="" alt="Imagem" class="imagem" />
          <div class="texto">
            <p class="nomes">Nome</p>
            <p class="detalhes">24 anos - Maringá - Paraná</p>
            <p class="detalhes">Salário R$ 4.200,00 - Gerente RH</p>
          </div>
        </div>
        <div class="campo1">
          <h2 class="titulo">Atual : Gerente de Rh - Departamento X</h2>
          <li class="campo-texto">- Atual</li>
          <li class="campo-texto">Trabalhando em -</li>
        </div>
        <div class="campo1">
          <h2 class="titulo">Contato :</h2>
          <li class="campo-texto">Telefone :</li>
          <li class="campo-texto">Email :</li>
          <li class="campo-texto">Endereço :</li>
          <span class="linha-texto">______________ Numero:</span>
        </div>
        <div class="campo1">
          <h2 class="titulo">Informações pessoais :</h2>
          <li class="campo-texto">Nome completo :</li>
          <li class="campo-texto">Data de nascimento :</li>
          <li class="campo-texto">Cpf :</li>
          <li class="campo-texto">RG :</li>
          <li class="campo-texto">Histórico Profissional :</li>
          <li class="campo-texto">Número da Conta Bancária :</li>
          <li class="campo-texto">Agência Bancária :</li>
          <li class="campo-texto">Banco :</li>
        </div>
        <div class="campo1">
          <h2 class="titulo">Documentação :</h2>
          <li class="campo-texto">Documento de Identidade :</li>
          <li class="campo-texto">Passaporte :</li>
          <li class="campo-texto">Comprovante de Residência :</li>
          <li class="campo-texto">Carteira de Trabalho :</li>
          <li class="anexo-linha">
            <span class="linha-texto">______________</span>
            <input type="file" class="anexo-arquivo" />
          </li>
        </div>

        <div class="campo1">
          <h2 class="titulo">Formação acadêmica :</h2>
          <li class="campo-texto">Formado em :</li>
        </div>
        <div class="campo1">
          <h2 class="titulo">Informações de Saúde e Segurança :</h2>
          <li class="campo-texto">Alergias :</li>
          <li class="campo-texto">Condições Médicas :</li>
        </div>
        <div class="campo1">
          <h2 class="titulo">Contato de Emergência :</h2>
          <li class="campo-texto">Nome do Contato de Emergência :</li>
          <li class="campo-texto">Relação com o Contato :</li>
          <li class="campo-texto">Telefone do Contato de Emergência :</li>
        </div>
        <button class="custom-button" @click="onClick">^</button>
      </div>
    </div>
  </div>
</template>
<script></script>

<style scoped>
.nome1 {
  color: rgb(0, 0, 0);
  font-size: 20px;
  font-weight: 500;
  width: 180px;
  white-space: nowrap;
  overflow: hidden; 
  text-overflow: ellipsis;
}
.status{
  height: 12px;
  width: 12px;
  background-color: #33FB3B;
  border-radius: 50%;
  position: absolute;
  margin-left:52px;
  margin-top: 65px;
}
.funcao {
margin-top: 20px;
margin-left:30px;
}
.funcionarios {
  display: flex;
  align-items: center;

}
.photo {
  height: 50px;
  width: 50px;
  margin-right: 20px;
  margin-left:15px;
  margin-top: 15px;
  background-color: #6D7993;
  border-radius: 50%;
}
.cargo{
  color: rgb(0, 0, 0);
  font-size: 20px;
  font-weight: lighter;
  margin-bottom: 10px;
}
.textos {
  color: black;
}
.nomes {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 10px;
}
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  overflow-y: auto; /* Adicionando scroll apenas para o conteúdo principal */
}

.sidebar {
  width: 300px; /* Largura da barra lateral */
  height: 1350px;
  background-color: #d5d5d5; /* Cor cinza */
  float: right;
  overflow-y: auto;
  max-height: calc( 1350px - 20px);
  margin: 0; 
  padding: 0;
  top: 0;
  left: 0;
}
/* Adicionando estilo à barra de rolagem da barra lateral */
.sidebar::-webkit-scrollbar {
  width: 15px; /* Largura da barra de rolagem */
}

/* Mudando a cor da barra de rolagem da barra lateral */
.sidebar::-webkit-scrollbar-track {
  background: #293C6C; /* Cor do fundo da barra de rolagem */
}

/* Mudando a cor do indicador da barra de rolagem da barra lateral */
.sidebar::-webkit-scrollbar-thumb {
  background: #FFFFFF; /* Cor do indicador da barra de rolagem */
  border-radius: 10px; /* Borda do indicador */
}

/* Mudando a cor quando o mouse está sobre a barra de rolagem da barra lateral */
.sidebar::-webkit-scrollbar-thumb:hover {
  background: #CCCCCC; /* Cor do indicador quando o mouse está sobre ele */
}
.quadrado {
  background-color: #293c6c;
  width: 600px;
  height: 1400px;
  padding: 10px;
  position: relative;
  border-radius: 20px;
}

.quadrado::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: #1f05c0;
  opacity: 0.2;
  border-radius: 20px;
}

.conteudo {
  display: flex;
  align-items: center;
  margin-left: 30px;
}

.imagem {
  height: 100px;
  width: 100px;
  margin-right: 20px;
  margin-top: 20px;
  background-color: #1235ae;
  border-radius: 50%;
}

.texto {
  color: white;
}

.nome {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 10px;
}

.detalhes {
  font-size: 18px;
  margin-bottom: 5px;
}

.campo1 {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  margin-top: 10px;
  margin-left: 40px;
}

.titulo {
  color: white;
  font-weight: bold;
}

.campo-texto {
  color: white;
  margin-top: 8px;
  margin-left: 30px;
}
.linha-texto {
  color: white;
  margin-top: 8px;
  margin-left: 50px;
}
.anexo-linha {
  display: flex;
  align-items: center;
}

.anexo-linha .anexo-arquivo {
  margin-left: 15px;
  color: white;
}
.campo1 li {
  list-style-type: none;
}
.custom-button {
  width: 80%;
  height: 30px;
  border: 2px solid white;
  background-color: transparent;
  color: white;
  font-size: 15px;
  padding: 8px 16px;
  cursor: pointer;
  transition: background-color 0.2s, transform 0.2s;
  border-radius: 20px;
  margin-top: 30px;
  margin-left: 10%;
}

.custom-button:active {
  transform: scale(2.95);
}
::-webkit-scrollbar {
  width: 15px; 
}

::-webkit-scrollbar-track {
  background: #293C6C;
}

::-webkit-scrollbar-thumb {
  background: #FFFFFF;
  border-radius: 10px; 
}

::-webkit-scrollbar-thumb:hover {
  background: #CCCCCC;
}
</style>
