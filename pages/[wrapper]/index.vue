<script setup lang="ts">

// macro to unset the layout
definePageMeta({ 
  layout:false
})

const layoutState = useState('layout',()=>'default')
const params = useRoute().params
const layout = params.wrapper
layoutState.value = layout 
onMounted(() => {
  console.log(`index onMounted called with layout ${layout}`)
})

onUpdated(() => {
  console.log('index onUpdated called')
})
</script>
<template>
  <Nav>
</template>