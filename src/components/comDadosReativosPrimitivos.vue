<template>
    <div class="componente">
        <h1>Componete com Dados Reativos Primitivos</h1>
        <p>Nome: {{ nome }} | Idade: {{ idade }}</p>
        <button v-on:click="fazerAniversario">Fazer Aniversário</button>
        <button v-on:click="mudarNome">Mudar Nome</button>
    </div>
</template>

<style>

</style>

<script setup>
import { ref } from 'vue';
    const nome = ref ("Dom")
    const idade = ref(41) 

    function fazerAniversario(){
        idade.value +=1
    }

    function mudarNome(){
        nome.value = "Dom Matos"
    }
</script>