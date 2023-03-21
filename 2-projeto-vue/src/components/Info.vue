<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades.</p>
        <p>Utilizo as seguintes tecnologias para front-end:</p>
        <ul>
            <li v-for="(technology, index) in frontend_technologies" v-bind:key="index">{{ technology}}</li>
        </ul>
        <p>Utilizo as seguintes tecnologias para back-end:</p>
        <ul>
            <li v-for="technology in backend_technologies" :key="technology.id">{{ technology.language }}</li>
        </ul>
        <div>
            <button @click="showEmail">{{ textoBotao }}</button>
        </div>
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p>Para acessar meu portifolio basta clicar <a v-bind:href="meu_link" target="_blank">Aqui!</a></p>
        <Picture />
    </div>
</template>
<script>
import Picture from "./Picture"

export default {
    name: "Info",
    components: {
        Picture
    },
    data() {
        return {
            esta_trabalhando: true,
            mostrar_email: true,
            email: "ericfreitassamp@gmail.com",
            meu_link: "https://ueriic.github.io/",
            textoBotao: "Mostrar e-mail",
            frontend_technologies: ["HTML", "CSS", "SCSS", "JavaScript", "Vue.js"],
            backend_technologies: [
                {id: 1, language: "TypeScript"},
                {id: 2, language: "Python"},
                {id: 3, language: "PHP"},
            ]
        }
    },
    methods: {
        showEmail() {
            this.mostrar_email = !this.mostrar_email
            if (!this.mostrar_email) {
                this.textoBotao = 'Mostrar e-mail'
            } else {
                this.textoBotao = 'Esconder e-mail'
            }
        }
    }
}
</script>