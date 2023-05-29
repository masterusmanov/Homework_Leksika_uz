<template>
  <div class="bg-green-50 pt-10">
    <main class="min-h-screen">
      <div class="mt-10">
        <BtnSearch titleq="ENG ⇆ UZB" @search="sendReq" />
        <div v-if="words !=''" class="mt-20">
          <Search :data="words"  />
        </div>
        <div v-else-if="errorMessage" class="mt-10">
          <ErrorEng />
        </div>
        <div v-else class="mt-10">
          <StartWords titles="Search any words, and we found this word defination, translation andetc."/>
        </div>
      </div>
    </main>
  </div>
</template>

<script setup>
import BtnSearch from "../components/BtnSearch.vue";
import { ref } from "vue";

const words = ref([]);
const errorMessage = ref("");


const sendReq = async (word) => {
  const { data } = await useFetch(
    `https://api.dictionaryapi.dev/api/v2/entries/en/${word}`
  );
  console.log(data.value);
  if (data.value) {
    words.value = data.value[0];
  } else {
    words.value = '';
    errorMessage.value = "error";
  }
};


useHead({
  title: `ENG ⇆ UZB page of Leksika.uz`,
  meta: [
    {
      name: "description",
      content: `ENG ⇆ UZB page of Leksika.uz`,
    },
    {
      name: "author",
      content: "Leksika.uz",
    },
  ],
});
</script>

<style lang="scss" scoped></style>
