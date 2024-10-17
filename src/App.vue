<script setup>
import { ref, computed } from 'vue'

const firstNumber = ref(null)
const secondNumber = ref(null)
const operation = ref('')

const result = computed(() => {
  const num1 = parseFloat(firstNumber.value)
  const num2 = parseFloat(secondNumber.value)

  if (isNaN(num1) || isNaN(num2)) {
    return ''
  }

  switch (operation.value) {
    case 'Multiplicação':
      return num1 * num2
    case 'Divisão':
      return num2 !== 0 ? num1 / num2 : 'Erro: Divisão por zero'
    case 'Soma':
      return num1 + num2
    case 'Subtração':
      return num1 - num2
    default:
      return ''
  }
})
</script>

<template>
  <div class="d-flex flex-column align-items-center">
    <header>
      <h1 class="mb-4 mt-3 text-center">Calculadora Aritmética</h1>
    </header>
    <div>
        <input v-model="firstNumber" class="text-center form-control mb-3" type="text" placeholder="Primeiro número">
        <input v-model="secondNumber" class="text-center form-control mb-3" type="text" placeholder="Segundo número">
        <select v-model="operation" class="form-control text-center mb-3">
          <option value="" disabled>Selecione a operação</option>
          <option value="Multiplicação">Multiplicação</option>
          <option value="Divisão">Divisão</option>
          <option value="Soma">Soma</option>
          <option value="Subtração">Subtração</option>
        </select>
        <p v-if="result !== ''">Resultado: {{ result }}</p>
    </div>
  </div>
</template>

<style scoped>
  /* Adicione seus estilos aqui, se necessário */
</style>
