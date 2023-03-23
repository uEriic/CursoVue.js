<template>
  <div>
    <Header :esta_logado=true />
    <PrimeiroComponente />
    <p>O dado do app é: {{ testando }}</p>
    <LifeCycle />
    <Pessoa />
  </div>
</template>

<script>
  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import Pessoa from './components/Pessoa.vue'
  import Header from './components/Header.vue'
  

  export default {
    name: "App",
    components: {
      PrimeiroComponente,
      LifeCycle,
      Pessoa,
      Header
    },
    data() {
      return {
        testando: "Teste"
      }
    }
  }
</script>
<style scoped>
* { 
  font-family: Arial, Helvetica, sans-serif;
  font-size: 18px;
  padding: 5px;
}
</style>