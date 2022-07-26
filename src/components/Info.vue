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
    </div>
</template>

<script>
    export default {
        name: 'Info',
        data() {
            return {
                trabalhando: false,
                estudando: true
            }
        }
    }
</script>