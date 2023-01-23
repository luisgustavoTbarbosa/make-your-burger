<template>
  <div>
    <p>Componente de mensagem</p>
    <div>
      <form id="burger-form">
        <div class="input-container">
          <label for="nome">Nome do cliente:</label>
          <input type="text" id="nome" name="nome" v-model="nome" placeholder="Luís Gustavo">
        </div>

        <div class="input-container">
          <label for="pao">Escolha o pão:</label>
          <select name="pao" id="pao" v-model="pao">
            <option value="">Selecione o seu pão</option>
            <option value="Integral">Integral</option>
          </select>
        </div>

         <div class="input-container">
          <label for="carne">Escolha a carne:</label>
          <select name="carne" id="carne" v-model="carne">
            <option value="">Selecione o tipo de carne</option>
            <option value="maminha">Maminha</option>
          </select>
        </div>

        <div id="opcionais-container" class="input-container">
          <label id="opcionais-title" for="opcionais">Selecione os opcionais:</label>
          <div class="checkbox-container">
            <input type="checkbox" name="opcionais" v-model="opcionais" value="salame">
            <span>Salame</span>
          </div>
        </div>

        <div class="input-container">
          <input type="submit" value="Criar meu Burger" class="submit-btn">
        </div>
      </form>
    </div>
  </div>
</template>

<script>
  name: 'BurgerForm'
</script>

<style scoped>
  #burger-form {
    width: 400px;
    margin: 0 auto;
  }

  .input-container {
    display: flex;
    flex-direction: column;
    margin-bottom: 20px;
  }

  label {
    margin-bottom: 15px;
    padding: 5px 10px;
    border-left: 4px solid #fcba03;
    color: #222;
    font-weight: bold;
  }

  input, select {
    width: 300px;
    padding: 5px 10px;
  }

  #opcionais-container {
    flex-direction: row;
    flex-wrap: wrap;
  }

  #opcionais-title {
    width: 100%;
  }

  .checkbox-container {
    display: flex;
    align-items: flex-start;
    width: 50%;
    margin-bottom: 5px;
  }

  .checkbox-container span,
  .checkbox-container input {
    width: auto;
  }

  .checkbox-container span {
    margin-left: 6px;
    font-weight: bold;
  }

  .submit-btn {
    margin: 0 auto;
    padding: 10px;
    background: #222;
    border: 2px solid #222;
    color: #fcba03;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
    transition: .5s;
  }

  .submit-btn:hover {
    background: transparent;
    color: #222;
  }
</style>