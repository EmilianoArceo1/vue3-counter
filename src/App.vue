<script>

export default {
    data: () => ({
        contador: 10,
    }),
    methods: {
        incrementar(){
            this.contador++;
        },

        decrementar(){
            this.contador--;
        },

        reset(){
            this.contador = 10;
        }
    }
};

</script>

<template>
    <div class="container">
        <img src ="./assets/logo.svg" alt="logo vue" width="125" height="125">
        <small><h1>Hola Mundo desde Vue.js 3</h1></small>
        <hr/>
        <h2>Contador: {{ contador }}</h2>
        <button @click="incrementar()">+1</button>
        <button @click="decrementar()">-1</button>
        <button @click="reset()">Reset</button>
    </div>
</template>

<style scoped>
    small{
        color: #666;
    }
    .container{
        text-align: center;
    }
    h1{
        font-weight: bolder;
    }
    h2{
        font-size: 2.5rem;
    }
    button{
        cursor: pointer;
        font-size: 1.5rem;
        margin: 0px 6px;
    }
</style>