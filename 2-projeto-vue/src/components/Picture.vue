<template>
    <img :src="avatar" :alt="descricao">
</template>
<script>
export default {
    name: "Picture",
    data() {
        return {
            avatar: "/imgs/avatar.png",
            descricao: "Eric Freitas"
        }
    }
}
</script>