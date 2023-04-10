<script setup>
import { ref } from 'vue'

const nome = ref('')
const senha = ref('')
const senhaConfirmar = ref('')
const data = ref(0)
const endereço = ref('')
const cidade = ref('')
const estado = ref('')
const hobbies = ref('')
const linguagemP = ref('')
const biografia = ref('')
const enviar = ref(false)





</script>

<template>
<div class="container">
    <div class="info">
<form action="">
    <p>Nome:</p>
    <input type="text" v-model="nome" placeholder="Nome" required/>
    <p>Senha</p>
    <input type="password" v-model="senha" placeholder="Senha" required/>
    <p>Confirmar senha</p>
    <input type="password" v-model="senhaConfirmar" placeholder="Confirmar senha" required/>
    <p>Data de nascimento</p>
    <input type="date" v-model="data" placeholder="Data de Nascimento" required/>
    <p>Endereço</p>
    <input type="text" v-model="endereço" placeholder="Endereço" required/>
    <p>Cidade</p>
    <input type="text" v-model="cidade" placeholder="Cidade" required/>
    <p>Estado</p>
    <select v-model="estado" placeholder="AC">
    <option value="AC">AC</option>
    <option value="AL">AL</option>
    <option value="AP">AP</option>
    <option value="AM">AM</option>
    <option value="BA">BA</option>
    <option value="CE">CE</option>
    <option value="DF">DF</option>
    <option value="ES">ES</option>
    <option value="GO">GO</option>
    <option value="MA">MA</option>
    <option value="MT">MT</option>
    <option value="MS">MS</option>
    <option value="MG">MG</option>
    <option value="PA">PA</option>
    <option value="PB">PB</option>
    <option value="PR">PR</option>
    <option value="PE">PE</option>
    <option value="PI">PI</option>
    <option value="RJ">RJ</option>
    <option value="RN">RN</option>
    <option value="RS">RS</option>
    <option value="RO">RO</option>
    <option value="RR">RR</option>
    <option value="SC">SC</option>
    <option value="SP">SP</option>
    <option value="SE">SE</option>
    <option value="TO">TO</option>
  </select>
  <p style="white-space: pre-line;">Hobbies</p>
  <textarea v-model="hobbies"/>
  <p>Linguagem de Programação</p>
  <input class="radioCss" type="radio" v-model="linguagemP" value="JavaScript" /> JavaScript
  <input class="radioCss" type="radio" v-model="linguagemP" value="Python" /> Python
  <input class="radioCss" type="radio" v-model="linguagemP" value="C" /> C#
  <input class="radioCss" type="radio" v-model="linguagemP" value="Php" /> Php
  <input class="radioCss" type="radio" v-model="linguagemP" value="SQL" /> SQL
  <input class="radioCss" type="radio" v-model="linguagemP" value="R" /> R
  <input class="radioCss" type="radio" v-model="linguagemP" value="VBA" /> VBA
  <p style="white-space: pre-line;">Biografia</p>
  <textarea v-model="biografia"/>
  <hr>
  <button type="submit" @click="enviar = !enviar">Salvar informações</button>
  <div v-if="enviar">
    {{ nome }}
  </div>
</form>
</div>
    <!-- div .container -->
</div>
</template>

<style scoped>
.container {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 50px;
}
button {
  font-weight: bold;
  margin: 0 50px;
  background-color: black;
  color: white;
  border: none;
  border-radius: 5px;
  padding: 15px 50px;
  cursor: pointer;
}
.cor1{
  color: green;
  font-weight: bold;
  margin: 50px 50px 50px 50px;
  background-color: black;
  border: none;
  border-radius: 5px;
  padding: 5px 10px;
}
.cor2{
  color: red;
  font-weight: bold;
  margin: 50px 50px 50px 50px;
  background-color: black;
  border: none;
  border-radius: 5px;
  padding: 5px 10px;
}
.estilo{
  font-weight: bold;
  margin: 50px 50px 50px 50px;
  background-color: black;
  border: none;
  border-radius: 5px;
  padding: 5px 10px;
  text-align: center;
  width: 50%;
}
.info {
  background-color: rgba(35,12,22,1);
  padding: 20px 30px;
  color: rgb(183, 210, 219);
  border-radius: 10px;
  text-align: center;
  margin: 10px;
}
.green{
  color: darkgreen;
}
.white {
  color: white;
}
.red {
  color: red;
}
.black{
  color: black;
}
.border-radius{
  border-radius: 15px;
}
/* p{
  margin: 50px 50px 50px 50px;
  
} */
h1 {
  color: white;
  font-weight: bold;
  font-size: 1.5em;
}
p{
    margin: 15px 15px 15px 15px;
}
.radioCss{
    margin-left: 15px;
}
</style>
