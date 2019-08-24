<template>      
     <div>
         <input type="number" v-model="number.N1" />
         <input type="number"  v-model="number.N2" />
         <button type="button" v-on:click="Resultado(number.N1,number.N2)">
           Contador        
         </button>
        
     </div>               
</template>
<script>
    export default{
    data(){
    return {
        number: {
            N1: ' ',
            N2: ' ',
        },
        }
       },    
        methods: {
            Resultado(num1, num2) {
                var n1 = num1;
                var n2 = num2;
                var suma = parseInt(n1) + parseInt(n2); 
                alert('Resultado' + ' ' + suma)
            }
       }
    }
</script>

<style media=" screen ">

</style>