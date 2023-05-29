<template>
    <div @click="open" class="absolute w-full h-[180vh] bg-black bg-opacity-20 top-0 left-0 flex justify-center items-center px-8">
        <div class="p-10 bg-white self-start mt-[15%] max-w-screen-md max-h-screen-xl">
            <h1 class="text-2xl font-bold">Akbar Kholmuradov</h1>
            <p class="mt-5 text-justify">Having graduated the International Economic Relations department of the University of World Economy and Diplomacy in 2001, Akbar dedicated his later years to translation and localization. When working as a translator in various huge projects, he faced the difficulty in finding reliable sources that can be used in translation to/from Uzbek language, and as a result some books for English learners and translators were published</p>
            <p class="mt-5 text-justify">English-Uzbek-English dictionary (<span class="text-teal-700">book, app</span>)</p>
            <p class="mt-5 text-justify">English Grammar for Uzbek Learners (<span class="text-teal-700">book, app</span>)</p>
            <button @click="emitClose" class="text-white mt-8 box-decoration-clone bg-blue-700 py-2 px-6 rounded-[20px]">Close</button>
        </div>
    </div>
</template>

<script setup>
import { defineEmits } from 'vue';

const emit = defineEmits(['close']);

function emitClose() {
  emit('close');
}
</script>

<style lang="scss" scoped>
</style>