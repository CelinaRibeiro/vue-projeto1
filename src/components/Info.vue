<template>
    <div>
        <p v-if="trabalhando">Estou trabalhando no momento</p>
        <p v-else>Nao estou trabalhando</p>
        <p>Uilizo as seguintes tecnologias:</p>
        <ul>
            <li>Javascript</li>
            <li>PHP</li>
            <li>Python</li>
        </ul>
        <p v-if="estudando">Estou estudando.</p>
        <p v-else>Não estou estudando</p>
        <p>Acesse meu portfólio <a v-bind:href="clique" target="_blank">clique</a> </p>
        <Picture />
    </div>
</template>

<script>
    import Picture from './Picture.vue'

    export default {
        name: 'Info',
        components: {
            Picture
        },
        data() {
            return {
                trabalhando: false,
                estudando: true,
                clique: 'http://nucleosti.com.br'
            }
        }
    }
</script>