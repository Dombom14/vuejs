<template>
    <div class="componente">
    <h1>Componente com Dados</h1>
    <p>Nome:{{ nomeProduto }} - {{ codigoProduto }}</p>

</div>
</template>

<style>

</style>

<script setup>
    const nomeProduto = "Apontador"
    const codigoProduto = "#987"
    
</script>

<!---script-->
//options API //
//export default {
 //   data:function(){
 //       return{
//            nomeProduto: "Caderno",
//            codigoProduto: "#321"
//        }
// }
//}

//Composition API //
//export default{
  //  setup:function(){
//        const nomeProduto= "Lápis"
//        const codigoProduto = "791"
 //       return {nomeProduto, ////
 
// codigoProduto}
///    }
//}
<!---script--->