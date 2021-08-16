<template>
  <div>
    <h3>{{ dataAtual }} / {{ mesAtual }} / {{ anoAtual }}</h3>
  </div>
</template>

<script>
let data = new Date();
let dia = data.getDay();
let mes = data.getMonth();
let ano = data.getFullYear();
if(dia <10){
  dia = "0"+dia;
}
if(mes <10){
  mes= "0"+mes;
}
export default{

  data(){
    return{
        dataAtual: dia,
        mesAtual: mes,
        anoAtual: ano
        
    }
    

  }

}

</script>

<style>


</style>
