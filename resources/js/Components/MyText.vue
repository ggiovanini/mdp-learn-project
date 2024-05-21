<script setup>
import {ref} from "vue";

const props = defineProps({
    custom: {
        type: String,
        default: 'text-black'
    },
})

const color = ref(props.custom);

function manipularProp() {
    color.value = color.value === "text-red-800" ? "text-black" : "text-red-800";
}
</script>

<template>
    <p class="text-xl mt-5 cursor-pointer" :class="color" @click="manipularProp">
        <slot></slot>
    </p>
</template>

<style scoped>

</style>
