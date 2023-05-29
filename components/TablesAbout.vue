<template>
  <div class="mt-32">
    <div class="flex justify-between items-start">
      <div class="w-[30%]">
        <h1 class="text-xl font-bold text-teal-600">Book edition</h1>
      </div>
      <div class="w-[70%]">
        <p class="text-justify text-xl">
          To reverse the situation, it was decided to compile a large
          English-Uzbek-English dictionary and the work started back in 2003. 2
          years later, the
          <a  href="#" class="text-teal-600 font-bold">first edition </a>of the
          bilingual dictionary was published in G’afur G’ulom publishing house;
          it is still
          <a href="#" class="text-teal-600 font-bold">available </a> for sale
          online. Much attention was directed to the Uzbek-English part; even
          now, it is the most comprehensive and complete UZ-EN dictionary. A
          <a href="#" class="text-teal-600 font-bold">mobile app </a> for Android
          devices was launched based on the dictionary with ma jor update of the
          lexical database.
        </p>
      </div>
    </div>
    <div class="flex justify-between items-start mt-5">
      <div class="w-[30%]">
        <h1 class="text-xl font-bold text-teal-600">Website dictionary</h1>
      </div>
      <div class="w-[70%]">
        <p class="text-justify text-xl">
          However, we still desperately needed a high-quality online dictionary
          for English-Uzbek language pair that could cover both everyday and
          area-specific vocabulary. In September 2022, on the date of 31th
          anniversary of Independence of Uzbekistan, Leksika.uz was successfully
          launched. Leksika.uz has mainly been designed to give English learners
          of any level the help they need to read, speak and write English more
          effectively. It is also intended to assist translators and localizers
          by providing useful tips and rules of thumb; these can be found in
          Localization section.
        </p>
      </div>
    </div>
    <div class="flex justify-between items-start mt-5">
      <div class="w-[30%]">
        <h1 class="text-xl font-bold text-teal-600">Prospects</h1>
      </div>
      <div class="w-[70%]">
        <p class="text-justify text-xl">
          ● Russian-Uzbek-Russian dictionary section with largest database on
          the web;
        </p>
        <p class="text-justify text-xl mt-2">
          ● content for easier learning of English, including grammar, writing
          tips, learning new words;
        </p>
        <p class="text-justify text-xl mt-2">
          ● useful tips and motivational articles for freelancers;
        </p>
        <p class="text-justify text-xl mt-2">
          ● articles for localizers to Uzbek language, including intricacies of
          Uzbek grammar;
        </p>
        <p class="text-justify text-xl mt-2">● and much more.</p>
      </div>
    </div>
    <div class="flex justify-between items-start mt-5">
      <div class="w-[30%]">
        <h1 class="text-xl font-bold text-teal-600">Our team</h1>
      </div>
      <Modal @close="close" v-if="modal1" />
      <Modals @close="close" v-if="modal2" />
      <div class="w-[70%] flex justify-center items-center">
        <div @click="open" class="w-1/2">
          <nuxt-link to="#" class="w-[500px] h-[300px]"><img src="../public/Akbar.png" alt=""  /></nuxt-link>
        </div>
        <div @click="open1" class="w-1/2">
          <nuxt-link to="#"><img src="../public/Asqar.png" alt="" /></nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const modal1 = ref(false);
const modal2 = ref(false);

const open = () => {
  modal1.value = true;
};
const open1 = () => {
  modal2.value = true;
};

const close = () => {
  modal1.value = false;
  modal2.value = false;
};
</script>

<style lang="scss" scoped></style>
