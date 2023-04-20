<script setup lang="ts">
  import { useStoreCounter } from '../stores/counter';
  defineProps<{ msg: string }>()  
  const counter = useStoreCounter();

  // https://reffect.co.jp/vue/vue-pinia#DevtoolsStore
</script>



<template>
  <h3>{{ msg }}</h3>
  <p>Count:{{ counter.count }}</p>
</template>

<style scoped>
</style>
