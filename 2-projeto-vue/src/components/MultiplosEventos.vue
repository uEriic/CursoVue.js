<template>
    <div>
        <button @click="primeiro(txt1, $event), segundo(txt2, $event)">Ativar múltiplos eventos</button>
        <p>{{  multiplos_eventos }}</p>
    </div>
</template>
<script>
export default {
    name: 'MultiplosEventos',
    data() {
        return {
            multiplos_eventos: "",
            txt1: 'Primeiro evento ativado!',
            txt2: 'Segundo evento ativado!',
        }
    },
    methods: {
        primeiro(txt) {
            this.multiplos_eventos = this.txt1
        },
        segundo(txt) {
            setTimeout(() => this.multiplos_eventos = this.txt2, 500)
        }
    }
}
</script>
<style scoped>
div {
    margin: 0 auto;
    font-size: 20px;

}
</style>