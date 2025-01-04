<template>
    <nav>
        <p>{{layout}}</p>
        <NuxtLink to="/">To /</NuxtLink>
        <NuxtLink to="/app">To /app</NuxtLink>
        <NuxtLink to="/red">To /red</NuxtLink>
        <NuxtLink to="/blue">To /blue</NuxtLink>
    </nav>
</template>
<script lang="ts" setup>
const layout = useState('layout', ()=> 'default')
</script>