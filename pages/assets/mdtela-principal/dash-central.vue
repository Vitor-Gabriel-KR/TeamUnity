<template>
  <div class="divisor">
    <div class="caixa"></div>
    
    <div class="container">
    <div class="quadrado">
      <div class="conteudo">
        <img src="/imagens/juan.jpeg" alt="Imagem" class="imagem2"  />
        <img src="/imagens/DIlma.png" alt="Imagem" class="imagem3" />
        <img src="/imagens/kratos.png" alt="Imagem" class="imagem4"  />
        <img src="/imagens/Naruto.png" alt="Imagem" class="imagem5" />
        <img src="/imagens/YasuoCareca.png" alt="Imagem" class="imagem6" />
        <div class="texto">
          <p class="nomes">{{ dadosFuncionario.nome_completo }}</p>
          <p class="detalhes">{{ (dadosFuncionario.data_nascimento) }} anos - {{ dadosFuncionario.endereco_residencial }}</p>
          <p class="detalhes">Salário R$ {{ dadosFuncionario.salario }} - {{ dadosFuncionario.cargo }}</p>
        </div>
      </div>
      <div class="campo1">
        <h2 class="titulo">Atual: {{ dadosFuncionario.cargo }} - {{ dadosFuncionario.departamento }}</h2>
        <li class="campo-texto">Trabalhando em: {{ dadosFuncionario.trabalhando_em }}</li>
      </div>
      <div class="campo1">
        <h2 class="titulo">Contato :</h2>
        <li class="campo-texto">Telefone: {{ dadosFuncionario.telefone }}</li>
        <li class="campo-texto">Email: {{ dadosFuncionario.email }}</li>
        <li class="campo-texto">Endereço: {{ dadosFuncionario.endereco_residencial }}</li>
        <span class="linha-texto">______________ Numero: {{ dadosFuncionario.numero_casa }}</span>
      </div>
      <div class="campo1">
        <h2 class="titulo">Informações pessoais :</h2>
        <li class="campo-texto">Nome completo: {{ dadosFuncionario.nome_completo }}</li>
        <li class="campo-texto">Data de nascimento: {{ dadosFuncionario.data_nascimento }}</li>
        <li class="campo-texto">CPF: {{ dadosFuncionario.cpf }}</li>
        <li class="campo-texto">RG: {{ dadosFuncionario.rg }}</li>
        <li class="campo-texto">Histórico Profissional: {{ dadosFuncionario.historico_profissional }}</li>
        <li class="campo-texto">Número da Conta Bancária: {{ dadosFuncionario.numero_conta_bancaria }}</li>
        <li class="campo-texto">Agência Bancária: {{ dadosFuncionario.agencia_bancaria }}</li>
        <li class="campo-texto">Banco: {{ dadosFuncionario.banco }}</li>
      </div>
      <div class="campo1">
        <h2 class="titulo">Documentação :</h2>
        <li class="campo-texto">Documento de Identidade: {{ dadosFuncionario.documento_identidade }}</li>
        <li class="campo-texto">Passaporte: {{ dadosFuncionario.passaporte }}</li>
        <li class="campo-texto">Comprovante de Residência: {{ dadosFuncionario.comprovante_residencia }}</li>
        <li class="campo-texto">Carteira de Trabalho: {{ dadosFuncionario.carteira_trabalho }}</li>
      </div>
      <div class="campo1">
        <h2 class="titulo">Formação acadêmica :</h2>
        <li class="campo-texto">Formado em: {{ dadosFuncionario.formacao_academica }}</li>
      </div>
      <div class="campo1">
        <h2 class="titulo">Informações de Saúde e Segurança :</h2>
        <li class="campo-texto">Alergias: {{ dadosFuncionario.alergias }}</li>
        <li class="campo-texto">Condições Médicas: {{ dadosFuncionario.condicoes_medicas }}</li>
      </div>
      <div class="campo1">
        <h2 class="titulo">Contato de Emergência :</h2>
        <li class="campo-texto">Nome do Contato de Emergência: {{ dadosFuncionario.contato_emergencia_nome }}</li>
        <li class="campo-texto">Relação com o Contato: {{ dadosFuncionario.contato_emergencia_relacao }}</li>
        <li class="campo-texto">Telefone do Contato de Emergência: {{ dadosFuncionario.contato_emergencia_telefone }}</li>
      </div>
    </div>
      
    </div>
  </div>
    <button class="invbox2" @click="setId(2)"></button>
    <button class="invbox3" @click="setId(3)"></button>
    <button class="invbox4" @click="setId(4)"></button>
    <button class="invbox5" @click="setId(5)"></button>
    <button class="invbox6" @click="setId(6)"></button> 
    <div :class="{ funcionarios1: true, show: isVisible }">
        <img src="/imagens/YasuoCareca.png" alt="photo" class="photo1" />
        <p class="status1"></p>
        <div class="textos1">
          <p class="nome2">Yasuo Careca</p>
        </div>
      </div>
    <button class="invbox7" @click="showFuncionario"></button>
</template>

<script>

import imgJson from '@/imagens/imagens.json'; 

export default {
  data() {
    return {
      id: 4, 
      dadosFuncionario: {},
      isVisible: false
    };
  },
  mounted() {
    this.carregarDadosFuncionario();
  },
  methods: {
    carregarDadosFuncionario() {
      const idFuncionario = this.id;
      this.dadosFuncionario = imgJson.find(funcionario => funcionario.id === idFuncionario);
    },  
    showFuncionario() {
      this.isVisible = true;
    },
    setId(id) {
  this.id = id;
  if (id === 2) {
    document.querySelector('.imagem2').style.display = 'block';
    document.querySelector('.imagem3').style.display = 'none';
    document.querySelector('.imagem4').style.display = 'none';
    document.querySelector('.imagem5').style.display = 'none';
    document.querySelector('.imagem6').style.display = 'none';
  } else if (id === 3) {
    document.querySelector('.imagem2').style.display = 'none';
    document.querySelector('.imagem3').style.display = 'block';
    document.querySelector('.imagem4').style.display = 'none';
    document.querySelector('.imagem5').style.display = 'none';
    document.querySelector('.imagem6').style.display = 'none';
  } else if (id === 4) {
    document.querySelector('.imagem2').style.display = 'none';
    document.querySelector('.imagem3').style.display = 'none';
    document.querySelector('.imagem4').style.display = 'block';
    document.querySelector('.imagem5').style.display = 'none';
    document.querySelector('.imagem6').style.display = 'none';
  } else if (id === 5) {
    document.querySelector('.imagem2').style.display = 'none';
    document.querySelector('.imagem3').style.display = 'none';
    document.querySelector('.imagem4').style.display = 'none';
    document.querySelector('.imagem5').style.display = 'block';
    document.querySelector('.imagem6').style.display = 'none';
  } else if (id === 6) {
    document.querySelector('.imagem2').style.display = 'none';
    document.querySelector('.imagem3').style.display = 'none';
    document.querySelector('.imagem4').style.display = 'none';
    document.querySelector('.imagem5').style.display = 'none';
    document.querySelector('.imagem6').style.display = 'block';
  } else {

  }
  this.carregarDadosFuncionario();
}
  },
};
</script>



<style scoped>
.invbox2{
  top:57%;
  left:77%;
  position: absolute;
  background-color: #1235ae;
  height: 70px;
  width: 300px;
  opacity: 0;
}
.invbox3{
  top:69%;
  left:77%;
  position: absolute;
  background-color: #1235ae;
  height: 70px;
  width: 300px;
  opacity: 0;
}
.invbox4{
  top:81%;
  left:77%;
  position: absolute;
  background-color: #1235ae;
  height: 70px;
  width: 300px;
  opacity: 0;
}
.invbox5{
  top:93%;
  left:77%;
  position: absolute;
  background-color: #1235ae;
  height: 70px;
  width: 300px;
  opacity: 0;
}
.invbox6{
  top:106%;
  left:77%;
  position: absolute;
  background-color: #1235ae;
  height: 70px;
  width: 300px;
  opacity: 0;
  z-index: 1;
}
.invbox7{
  top:55%;
  left:15%;
  position: absolute;
  background-color: #1235ae;
  height: 30px;
  width: 90px;
  opacity: 0;
}
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
  background: rgb(9,9,121);
  background: linear-gradient(90deg, rgba(9,9,121,1) 44%, rgba(2,0,36,1) 100%);
  width: 600px;
  height: 1350px;
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

.imagem2 {
  height: 100px;
  width: 100px;
  margin-right: 20px;
  margin-top: 20px;
  background-color: #1235ae;
  border-radius: 50%;
  display: none;
}
.imagem3 {
  height: 100px;
  width: 100px;
  margin-right: 20px;
  margin-top: 20px;
  background-color: #1235ae;
  border-radius: 50%;
  display: none;
}
.imagem4 {
  height: 100px;
  width: 100px;
  margin-right: 20px;
  margin-top: 20px;
  background-color: #1235ae;
  border-radius: 50%;
}
.imagem5 {
  height: 100px;
  width: 100px;
  margin-right: 20px;
  margin-top: 20px;
  background-color: #1235ae;
  border-radius: 50%;
  display: none;
}
.imagem6 {
  height: 100px;
  width: 100px;
  margin-right: 20px;
  margin-top: 20px;
  background-color: #1235ae;
  border-radius: 50%;
  display: none;
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
.nome2 {
  color: rgb(0, 0, 0);
  font-size: 18px;
  font-weight: 500;
  width: 180px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  border-bottom: 1px solid  #727272;
}
.status1 {
  height: 11px;
  width: 11px;
  background-color: #33FB3B;
  border-radius: 50%;
  position: absolute;
  margin-left: 48px;
  margin-top: 45px;
}
.funcao1 {
  margin-top: 15px;
  margin-left: 25px;
}
.funcionarios1 {
  display: flex;
  position: absolute;
  top:103%;
  left:78%;
  width: 276px;
  height: 60px;
  align-items: center;
  border: 2px solid  #c5c5c5;
  border-radius: 10px;
  margin-top: 15px;
  cursor: pointer;
  opacity: 0;
  
}
.funcionarios1:hover {
  background-color: #ecce96;
}

.funcionarios1.show {
  opacity: 1;
}
.photo1 {
  height: 45px;
  width: 45px;
  margin-right: 12px;
  margin-left: 13px;
  background-color: #6D7993;
  border-radius: 50%;
  border: 2px solid #727272;
}
.cargo1 {
  color: rgb(0, 0, 0);
  font-size: 20px;
  font-weight: lighter;
  margin-bottom: 10px;
}
.textos1 {
  color: black;
}
</style>
