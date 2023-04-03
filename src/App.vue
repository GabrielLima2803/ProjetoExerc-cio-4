<script setup>
import { ref } from 'vue'

const nome = ref('')
const senha = ref('')
const senhaConfirmar = ref('')
const data = ref(0)

</script>

<template>
<div class="container">

<form action="">
    <input type="text" v-model="nome" placeholder="Nome" required/>
    <input type="password" v-model="senha" placeholder="Senha" required/>
    <input type="password" v-model="senhaConfirmar" placeholder="Confirmar senha" required/>
    <input type="date" v-model="data" placeholder="Data de Nascimento" required/>

</form>
    <!-- div .container -->
</div>
</template>

<style scoped>

</style>
