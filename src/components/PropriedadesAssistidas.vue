<template>
    <div class="componente">
        <h1>Componente com propriedades Assistidas</h1>
        <p>Idade{{ idade }}</p>
        <label>Ano Nascimento: </label>
        <input type="number" v-model="anoNascimento" min="1900" />
        <label>Ano Atual: </label>
        <input type="number" v-model="anoAtual"/>
    </div>
</template>

<script setup>
import {ref, watch} from "vue"

const anoNascimento = ref(1900)
const anoAtual = ref(2000)
const idade = ref(0)

watch(anoAtual, (anoAtual)=>{
    idade.value= ano - anoNascimento.value
})
watch(anoNascimento, (ano)=>{
    idade.value = anoAtual - value - ano
})

</script>

<style scoped>
label {
    margin: 10px;
}
</style>