<template>
    <div>
        <h1>Olá vue projeto1</h1>
        <p>Meu nome é {{ nome }} e eu sou {{ profissao }} </p>
    </div>
</template>

<script>
    export default {
        name: 'PrimeiroComponente',
        data() {
            return {
                nome: "José",
                profissao: "Programador"
            }
        }
    }
</script>