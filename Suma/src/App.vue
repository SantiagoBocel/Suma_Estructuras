<template>
    <div id="app">
        <h3>Santiago Bocel 1076818</h3>
        <h4>Instrucciones: Cambiar el simbolo por la operacion que se desea realizar y luego precionar el boton </h4>
        <h1>Operaciones de numeros</h1>
        <Suma/>
    </div>
</template>

<script>
    import Suma from './components/Suma.vue';
    export default {
        name: 'app',
        components: {
            Suma
        }
    }
</script>
<style>
</style>
