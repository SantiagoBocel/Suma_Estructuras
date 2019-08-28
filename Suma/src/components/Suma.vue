 <template>      
     <div>
         <h4>Numero 1</h4>
         <input type="number" v-model="number.N1" /><br /><h4>Simbolo</h4>
         <input type="text" v-model="number.Simbolo" /><br />
         <h4>Numero 2</h4>
         <input type="number"  v-model="number.N2" /><br />
         <button type="button" v-on:click="Resultado(number.N1,number.N2,number.Simbolo)">
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
            Simbolo: '+',
        },
        }
       },    
        methods: {
         
            Resultado(num1, num2, Simbolo) {
                var n1 = num1;
                var n2 = num2;
                var suma = parseInt(n1) + parseInt(n2);
                var Resta = parseInt(n1) - parseInt(n2);
                var Multiplicar = parseInt(n1) * parseInt(n2);
                var Divicion = parseInt(n1) / parseInt(n2);
                if (Simbolo == '+') {
                alert('Resultado' + ' ' + suma)
                }
                if (Simbolo == '-') {
                    alert('Resultado' + ' ' + Resta)
                }
                if (Simbolo == '*') {
                    alert('Resultado' + ' ' + Multiplicar)
                }
                if (Simbolo == '/') {
                    alert('Resultado' + ' ' + Divicion)
                }
            }
       }
    }
</script>

<style media=" screen ">

</style>