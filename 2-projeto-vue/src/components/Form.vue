<template>
    <form action="">
        <h2>Login</h2>
        <inputText />
        <inputText />
        <Submit />
    </form>
</template>

<script>
import Submit from './form/Submit.vue'
import inputText from './form/inputText.vue'

export default {
    name: 'Form',
    components: {
        inputText,
        Submit
    }
}
</script>