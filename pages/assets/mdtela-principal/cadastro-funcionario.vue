<template>
    <div class="container2">
        <p class="titulo">Dados Pessoais</p>
        <div class="model">
            <div class="area">
                <form>
                    <div class="horizontal-container">
                        <div class="formgrupo1">
                            <input class="tipo3" type="file" id="foto" name="foto" required>
                        </div>
                        <div class="formgrupo2">
                            <label class="categoria" for="name">Nome Completo</label>
                            <input class="tipo2" type="text" id="name" name="name" required>
                        </div>
                        <div class="formgrupo1">
                            <label class="categoria" for="CPF">CPF</label>
                            <input class="tipo1" id="CPF" name="CPF" required>
                        </div>

                    </div>
                    <div class="horizontal-container2">
                        <div class="formgrupo1">
                            <label class="categoria" for="dataNascimento">Data de Nascimento</label>
                            <input class="tipo1" id="dataNascimento" name="dataNascimento" required>
                        </div>
                        <div class="formgrupo1">
                            <label class="categoria" for="RG">RG</label>
                            <input class="tipo1" id="RG" name="RG" required>
                        </div>
                    </div>
                    <div class="horizontal-container">
                        <div class="formgrupo1">
                            <label class="categoria" for="dataNascimento">Data de Nascimento</label>
                            <input class="tipo1" id="dataNascimento" name="dataNascimento" required>
                        </div>
                        <div class="formgrupo1">
                            <label class="categoria" for="RG">RG</label>
                            <input class="tipo1" id="RG" name="RG" required>
                        </div>
                    </div>

                    <div class="horizontal-container">
                        <div class="formgrupo1">
                            <label class="categoria" for="estadoCivil">Estado Civil</label>
                            <input class="tipo1" id="estadoCivil" name="estadoCivil" required>
                        </div>
                        <div class="formgrupo1">
                            <label class="categoria" for="dependentes">Dependentes</label>
                            <input class="tipo1" id="dependentes" name="dependentes" required>
                        </div>
                    </div>

                    <div class="horizontal-container">
                        <div class="formgrupo1">
                            <label class="categoria" for="informacoesFiscais">Informações Fiscais</label>
                            <input class="tipo1" id="informacoesFiscais" name="informacoesFiscais" required>
                        </div>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

  
  <script>
 
  </script>
  
  <style scoped>
  .horizontal-container {
    display: flex;
    flex-direction: row;
}
.horizontal-container2 {
    display: flex;
    flex-direction: column;
}

   .formgrupo1{
    position: relative;
    display: flex;
    flex-direction: column;
    }
    .formgrupo2{
    position: relative;
    display: flex;
    flex-direction: column;
    }
    .tipo1{
    padding: 0 2px;
    width: 100px;
    height: 22px;
    border: 2px solid #d0cfff;
    background-color: transparent;
    margin: 0 10px 10px 10px;
    }
    .categoria{
    color: #323535 ;
    font-size: 14px;
    margin-top:10px;
    margin-left: 10px;
    margin-bottom: 2px;
    }
    .tipo2{
    padding: 0 2px;
    width: 250px;
    height: 22px;
    border: 2px solid #d0cfff;
    background-color: transparent;
    margin: 0 10px 10px 10px;
    }
    .tipo3{
    padding: 0 2px;
    width: 150px;
    height: 150px;
    border: 2px solid #d0cfff;
    background-color: #d0cfff;
    margin: 10px 10px 10px 10px;
    }
    .container2 {
    display: flex;
    position: relative;
    justify-content: center;
    align-items: center;
    margin-top: 30px;
    margin-left: 220px;
    }

    .titulo {
    width: 120px;
    height: 40px;
    border: 2px solid #323535;
    display: flex;
    justify-content: center;
    align-items: center;
    position: absolute;
    border-radius: 20px;
    bottom: 82%;
    left: 80px;
    margin-bottom: 60px;
    background-color: white;
    z-index: 1;
    }

    .model {
    width: 700px;
    height: 460px;
    border: 2px solid #323535;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    border-radius: 20px;
    background-color: transparent;
    }

    .area {
    width: 600px;
    height: 350px;
    border: 2px solid #d0cfff;
    background-color: transparent;
    }
</style>