<template>
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Projetos</a></li>
            <li><a href="#">Contato</a></li>
        </ul>
    </nav>
</template>
<script>
export default {
    name: "Header"
}
</script>
<style scoped>
    ul {
        display: flex;
        align-items: center;
        justify-content: space-around;
        list-style: none;
        display: flex;
        background-color: #888;
    }
    li {
        margin-right: 10px;
    }
    a {
        color: #fbfbfb;
        text-decoration: none;
        transition: .5s;
    }
    a:hover {
        transform: scale(1.3);
        color: turquoise;
    }
</style>