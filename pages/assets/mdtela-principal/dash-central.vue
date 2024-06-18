<template>
  <div class="divisor">
    <div class="caixa"></div>
    
    <div class="container">
      <div class="quadrado" :style="{ height: quadradoHeight + 'px' }">
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
        <button class="custom-button" v-if="primeiroBotaoVisivel" @click="alterarTamanho">\/</button>
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
        <button class="custom-button" v-if="!primeiroBotaoVisivel" @click="alterarTamanho">\/</button>
      </div>
      
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      quadradoHeight: 520,
      primeiroBotaoVisivel: true
    };
  },
  methods: {
    alterarTamanho() {
      if (this.quadradoHeight === 520) {
        this.quadradoHeight = 1450;
        this.primeiroBotaoVisivel = false;
      } else {
        this.quadradoHeight = 520;
        this.primeiroBotaoVisivel = true;
      }
    }
  }
};
</script>
<style scoped>
.caixa{
  margin-bottom: 15px;
}
.container {
  display: flex;
  position: relative; 
  justify-content: center;
  align-items: center;
  margin-top: 50px;
  margin-left: 220px;
}

.quadrado {
  background: rgb(195,119,34);
  background: linear-gradient(0deg, rgba(195,119,34,1) 0%, rgba(174,104,54,1) 7%, rgba(156,91,71,1) 16%, rgba(136,77,90,1) 28%, rgba(117,63,108,1) 43%, rgba(92,45,132,1) 65%, rgba(69,29,154,1) 100%);
  width: 600px;
  height: 520px;
  padding: 10px;
  position: relative;
  border-radius: 20px;
  overflow: hidden;
  transition: height 0.5s ease-in-out;
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

.nomes {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 6px;
}

.detalhes {
  font-size: 18px;
  margin-bottom: 2px;
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
  color: rgb(255, 255, 255);
  margin-top: 8px;
  font-size: 17px;
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

.custom-button:hover {
  background-color: rgba(255, 255, 255, 0.1);
}

.custom-button:active {
  transform: scale(0.95);
}

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
  background: #CCCCCC;
}
</style>