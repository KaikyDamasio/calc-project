<script setup>

</script>

<template>
  <body>
    <header>
      <h1 class="mb-4 mt-3 text-center">Calculadora Aritmética</h1>
    </header>
    <div class="d-flex flex-column align-items-center">
    <div class="d-flex flex-column">
      <div class="d-flex flex-row mb-3">
        <input class="text-center form-control" type="text" placeholder="Primeiro número">
      </div>
      <div class="d-flex flex-row mb-3 gap-4">
        <input class="text-center form-control" type="text" placeholder="Segundo número">
      </div>
      <div class="d-flex flex-row mb-3">
        <select class="form-control text-center" value="">
          <option value="" disabled selected>Selecione a operação</option>
          <option value="Multiplicação">Multiplicação</option>
          <option value="Divisão">Divisão</option>
          <option value="Soma">Soma</option>
          <option value="Subtração">Subtração</option>
        </select>
      </div>
    </div>
  </div>
  </body>

</template>

<style scoped></style>
