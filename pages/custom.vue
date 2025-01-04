<script setup lang="ts">
const layout = useState('layout')

onMounted(() => {
  console.log(`index onMounted called with layout ${layout.value}`)
})
onUpdated(() => {
  console.log('custom onUpdated called')
})

</script>
<template>
  <p>Custom.</p>
  <NuxtLink to="/">To index</NuxtLink>
</template>
