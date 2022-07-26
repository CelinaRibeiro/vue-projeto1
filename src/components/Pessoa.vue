<template>
    <div>
        <h1>Meu nome é {{ nome }}</h1>
        <Info />
        <Form /> 
    </div>
</template>

<script>
    import Info from './Info'
    import Form from './Form'

    export default {
        name: 'Pessoa',
        components: {
            Info,
            Form
        },
        data() {
            return {
                nome: "Maria"
            }
        }
    }
</script>