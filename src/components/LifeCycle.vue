<template>
    <div>
        <h1>Meu nome é {{ nome }} </h1>
    </div>
</template>

<script>
    export default {
        name: 'LifeCycle',
        data() {
            return {
                nome: 'Ainda nao sei'
            }
        },
        created() {
            setTimeout(() => {
                this.nome = 'Mateus'
            }, 1000)
            
        },
        mounted(){
            setTimeout(() => {
                this.nome = 'Pedro'
            }, 2000)
           
        }
    }
</script>