<template>
  <div class="elemento">
    <h2>Dados Cliente</h2>
    <p>Nome: {{ nome }}</p>
    <button style="margin-bottom: 10px;" @click="alterarNome">Alterar nome</button>
  </div>
</template>

<script>
export default {
  name: "dados-cliente",
  props: {
    nome: String
  },
  methods: {
    alterarNome() {
      this.$emit('eventoPersonalizado', 'Joana')
    }
  }

}
</script>

<style>
.elemento {
  flex: 1;
  border: 2px solid #fff;
  color: #fff;
}
</style>