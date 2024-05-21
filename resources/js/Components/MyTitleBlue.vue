<script setup>
import {ref} from "vue";
import MyTitle from "@/Components/MyTitle.vue";

const visual = ref(true);
const number = ref(0);

function trocarTexto() {
    visual.value = !visual.value;
    number.value++;
}
</script>

<template>
    <MyTitle custom="text-blue-800" @click="trocarTexto">
        <span v-if="visual">
            <slot></slot>
        </span>
        <span v-else>
            Clicado {{ number }}
        </span>
    </MyTitle>
</template>

<style scoped>

</style>
