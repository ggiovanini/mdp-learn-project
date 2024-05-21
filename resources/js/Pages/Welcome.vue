<script setup>
import { Head } from '@inertiajs/vue3';
import MyTitle from "@/Components/MyTitle.vue";
import MyTitleBlue from "@/Components/MyTitleBlue.vue";
import FontItalicoEspecial from "@/Components/FontItalicoEspecial.vue";
import MyText from "@/Components/MyText.vue";
</script>

<template>
    <Head title="Welcome" />
    <MyTitleBlue>Foo</MyTitleBlue>
    <MyTitle
        custom="text-gray-200"
    >
        Outra <FontItalicoEspecial>Algo</FontItalicoEspecial> COisa
    </MyTitle>
    <MyTitle>Outra coisa</MyTitle>

    <MyText>Dasd fasdfasdf sadf sdafasdfasd fasd </MyText>
    <MyText> fasd fasdfasdf sadf sdafasdfasd fasd </MyText>
    <MyText>Fasd asdf sadf sdafasdfasd fasd </MyText>
    <MyText> fasd fasdfasdf sadf sdafasdfasd fasd </MyText>
    <MyText> fasd fasdfasdf sadf sdafasdfasd fasd </MyText>
    <MyText> fasd fasdfasdf sadf sdafasdfasd fasd </MyText>
</template>
