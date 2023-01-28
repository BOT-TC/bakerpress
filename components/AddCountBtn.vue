<script setup>
import { ref } from 'vue'

const counter = ref(0)

function bump() {
  counter.value++
}
</script>

<template>
  <div>
    <button @click="bump">: {{ counter }} :</button>
  </div>
</template>
