<template>
    <nav>
        <router-link to="/" id="logo-url">
            <img :src="logo" :alt="alt" id="logo">
        </router-link>
        <router-link to="/">Home</router-link>
        <router-link to="/pedidos">Pedidos</router-link>
    </nav>
</template>
<script>
export default {
    name: 'Navbar',
    props: {
        logo: String,
        alt: String
    }
}
</script>
<style scoped>
    nav {
        background-color: #222;
        border-bottom: 4px solid #111;
        padding: 15px 50px;
        display: flex;
        justify-content: space-around;
        align-items: center;
        gap: 5rem;
    }
    nav #logo-url {
        margin: auto;
        margin-left: 0;
    }
    #logo {
        width: 48px;
        height: 48px;
    }
    nav a {
        color: #fcba03;
        text-decoration: none;
        transition: .6s;
        font-size: 24px;
    }
    nav a:hover {
        color: white;
        transform: scale(1.1);
    }
</style>