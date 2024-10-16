<script setup>

</script>

<template>
    <div class="d-flex flex-column align-items-center">
      <header>
      <h1 class="mb-4 mt-3">Calculadora Aritmética</h1>
      </header>
      <div class="col-md-3 mb-3">
        <input class="text-center form-control" type="text" placeholder="Primeiro número">
      </div>
      <div class="col-md-3 mb-3">
        <input class="text-center form-control" type="text" placeholder="Segundo número">
      </div>
      <div class="col-md-3 mb-3">
        <select class="form-control text-center" value="">
          <option value="" disabled selected>Selecione a operação</option>
          <option value="Multiplicação">Multiplicação</option>
          <option value="Divisão">Divisão</option>
          <option value="Soma">Soma</option>
          <option value="Subtração">Subtração</option>
        </select>
      </div>
    </div>
</template>

<style scoped>

</style>
