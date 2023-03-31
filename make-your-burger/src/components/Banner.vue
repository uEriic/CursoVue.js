<template>
    <div id="main-banner">
        <h1>Make Your Banner</h1>
    </div>
</template>
<script>
export default {
    name: 'Banner'
}
</script>
<style scoped>
#main-banner {
    background-image: url('../assets/burger.jpg');
    background-position: 0 -250px;
    background-size: cover;
    height: 600px;
    display: flex;
    justify-content: flex-start;
    align-items: center;
}
#main-banner h1 {
    color: white;
    text-align: center;
    font-size: 60px;
    background-color: #222;
    padding: 20px 40px;
}
</style>