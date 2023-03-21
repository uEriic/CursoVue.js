<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>Meu nome é {{ name }} e sou {{ job }}</p>
        <MultiplosEventos />
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'
export default {
    name: 'PrimeiroComponente',
    data() {
        return {
            name: "Eric",
            job: "Programming Student"
        }
    },
    components: {
        MultiplosEventos,
    }
}
</script>