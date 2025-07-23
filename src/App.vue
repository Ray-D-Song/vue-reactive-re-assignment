<script setup>
import { reactive } from 'vue'
import Form from './components/Form.vue'

const form = reactive({
  name: 'ray-d-song',
  age: 18
})
</script>

<template>
  <main>
    <Form v-model="form" />
    <h2>{{ form.name }}</h2>
    <h2>{{ form.age }}</h2>
  </main>
</template>
