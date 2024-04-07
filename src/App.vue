<script setup>
import { ref, shallowRef, computed, watch, nextTick } from 'vue'
import chart from 'chart.js/auto'

const weights = ref([])

const weightChartE1 = ref(null)

const weightChart = shallowRef(null)

const weightInput = ref(60.0)

const currentWeight = computed(() => {
  return weights.value.sort((a, b) => b.date - a.date)[0] || { weight: 0 }
})

</script>

<template>
  <h1>Hello, world!</h1>
</template>

<style scoped>

</style>
