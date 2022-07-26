<template>
    <img :src="bebida" :alt="descricao">
</template>

<script>
    export default {
        name: 'Picture',
        data() {
            return {
                bebida: './img/cat1.png',
                descricao: 'Suco'
            }
        }
    }
</script>