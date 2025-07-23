<script setup>
import { watch } from 'vue'

const modelValue = defineModel()

watch(modelValue.value, (newVal) => {
  console.log(newVal)
})
</script>

<template>
  <div>
    <input v-model="modelValue.name" />
    <input v-model="modelValue.age" type="number" />
  </div>
</template>
