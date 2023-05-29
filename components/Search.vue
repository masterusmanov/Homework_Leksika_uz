<template>
    <div class="container mx-auto  flex justify-center items-center p-10">
        <div class="w-[60%] h-[250px] bg-white pl-5 rounded-2xl shadow-lg shadow-teal-600 ">
            <div class="p-5">
                <h1 class="text-4xl font-bold">{{data.word}}</h1>
                <p class="text-xl pt-3 text-gray-500 ">{{data?.meanings?.map((i) => i?.partOfSpeech)?.join(", ") }}</p>
            </div>
            <div class="flex justify-beetwen items-center">
                <p @click="playAudio" class="ml-5 text-3xl cursor-pointer">🔊</p>
                <audio id="audio" :src="data?.phonetics[0]?.audio || data?.phonetics[1]?.audio"></audio>
                <p class="text-xl ml-7"> {{data?.phonetics?.find((i) => i?.text)?.text}}</p>
            </div>
            <div class="p-5">
                <p class="text-xl">{{data.word}}</p>
                <p class="pt-2">{{data?.meanings?.find((i) => i?.definitions?.find((j) => j?.example))?.definitions?.find((e) => e?.example)?.example}}</p>
            </div>
        </div>
    </div>
  </template>
  
  <script setup>
    const props = defineProps(["data"])
        console.log(props);
    const playAudio = () => {
        const audio = document.getElementById("audio");
        audio.play();
    };
    
    
  </script>
  
  <style lang="scss" scoped></style>