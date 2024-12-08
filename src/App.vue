<script setup>

import PrimeiroComponente from "./components/PrimeiroComponente.vue"
import ComDados from "./components/ComDados.vue"
import ComDadosReativosPrimitivos from "./components/comDadosReativosPrimitivos.vue";
import ComDadosReativosNaoPrimitivos from "./components/comDadosReativosNaoPrimitivos.vue";
import DataBinding from "./components/DataBinding.vue";
import ComProps from "./components/ComProps.vue";
import EscutaEvento from "./components/EscutaEvento.vue";


</script>

<template>
  <header>Vue</header>
  <EscutaEvento />
  <ComProps item="Caneta" v-bind:preco= "4.50" />
  <ComProps item="Caderno" v-bind:preco= "12.00" />
  <ComProps item="Abondador" :preco="3.50" />
  <DataBinding />
  <ComDadosReativosPrimitivos />
  <ComDadosReativosNaoPrimitivos />
  <ComDados />
  <PrimeiroComponente />
</template>

<style scoped>

</style>