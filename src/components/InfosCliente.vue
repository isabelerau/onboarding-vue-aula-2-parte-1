<template>
  <div class="elemento">
    <h2> Infos Cliente</h2>
    <p> Nome: {{ nome }}</p>
    <button class="btn" @click="reiniciar"> Reiniciar nome</button>
  </div>
</template>

<script>
export default {
  name: 'infos-cliente',
  props: {
    nome: String,
    reiniciar: Function
  }
}
</script>

<style scoped>
.btn {
  margin-bottom: 20px;
}

</style>