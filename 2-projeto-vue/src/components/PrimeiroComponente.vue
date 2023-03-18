<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>Meu nome é {{ name }} e sou {{ job }}</p>
    </div>
</template>

<script>
export default {
    name: 'PrimeiroComponente',
    data() {
        return {
            name: "Eric",
            job: "Programming Student"
        }
    }
}
</script>