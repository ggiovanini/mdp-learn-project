<script setup>
defineProps({
    custom: {
        type: String,
        default: 'text-pink-800'
    },
})
</script>

<template>
    <h1 class="font-medium text-6xl" :class="custom">
        <slot></slot>
    </h1>
</template>

<style scoped>

</style>
