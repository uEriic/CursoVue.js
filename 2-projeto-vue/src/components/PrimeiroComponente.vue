<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>Meu nome é {{ name }} e sou {{ job }}</p>
        <MultiplosEventos />
        <ReutilizacaoVue/>
        <ReutilizacaoVue/>
        <ReutilizacaoVue/>
        <ReutilizacaoVue/>
        <ReutilizacaoVue/>
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'
import ReutilizacaoVue from './Reutilizacao.vue'
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
        ReutilizacaoVue
    }
}
</script>