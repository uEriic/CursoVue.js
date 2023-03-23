<template>
    <div>
        <img :src="avatar" :alt="descricao">
        <MudarImagem @mudar-imagem="trocarImagem" />
    </div>
</template>
<script>
import MudarImagem from './MudarImagem.vue'

export default {
    name: "Picture",
    data() {
        return {
            avatar: "/imgs/avatar.png",
            descricao: "Eric Freitas"
        }
    },
    components: {
        MudarImagem
    },
    methods: {
        trocarImagem() {
           if (this.avatar === "/imgs/avatar.png") {
            this.avatar = "/imgs/avatar2.png"
           } else{
            this.avatar = "/imgs/avatar.png"
           }
        }
    }
}
</script>