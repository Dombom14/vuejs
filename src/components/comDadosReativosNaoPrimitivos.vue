<template>
    <div class="componente">
        <h1>Componete com Dados Reativos Não Primitivos</h1>
        <p>Nome: {{ pessoa.nome }} | Idade: {{ pessoa.idade }}</p>
        <button @click="fazerAniversario">Fazer Aniversário</button>
        <button @click="mudarNome">Mudar Nome</button>
    </div>
</template>

<style>

</style>

<script setup>
import { reactive } from 'vue';

    const pessoa = reactive({nome: "dom", idade: 41})
 

    function fazerAniversario(){
        pessoa.idade +=1
    }

    function mudarNome(){
        pessoa.nome= "Dom Matos"
    }
</script>