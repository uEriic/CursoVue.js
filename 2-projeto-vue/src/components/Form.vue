<template>
    <div>
        <div>
            <h2>Login</h2>
        </div>
        <form @submit="enviarForm($event)">
            <div>
                <input type="text" v-model="name">
            </div>
            <div>
                <input type="text" v-model="email">
            </div>
            <div>
                <Submit />
            </div>
        </form>
    </div>
</template>

<script>
import Submit from './form/Submit.vue'
import inputText from './form/inputText.vue'

export default {
    name: 'Form',
    data() {
        return {
            name: '',
            email: ''
        }
    },
    components: {
        inputText,
        Submit
    },
    methods: {
        enviarForm(e) {
            e.preventDefault();
            const name = this.name;
            const email = this.email;

            console.log(`Formulário enviado! Nome: ${name} & ${email}`)
        }
    }
}
</script>