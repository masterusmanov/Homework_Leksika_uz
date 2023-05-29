<template>
    <div class="bg-green-50 pt-5 pb-5 ">
        <main class="container min-h-screen mx-auto">
            <div  class="flex">
                <div class="w-[100%]">
                     <div class="overflow-hidden bg-white rounded-[20px] p-14 w-[100%] mt-5">
                        <h1 class="text-center text-2xl font-bold">Remember the days when you couldn’t find the proper translation of an English word to the Uzbek language? I also know those feelings when you run against the lack of general use dictionaries - not to mention the specialized ones, a total absence of online resources in Uzbek, a pre-requisite of knowing the Russian language in order to apply indirect translation (EN RU UZ and vice versa).</h1>
                        <TablesAbout/>
                     </div>
                </div>
            </div>
            
        </main>
    </div>
  </template>
  
  <script setup>      
  const {name} = useRoute();
    useHead({
        title: `${name} page of Leksika.uz`,
        meta: [
        {
            name: "description", content: `${name} page of Leksika.uz`
        },
        {
            name: "author", content: "Leksika.uz"
        }
        ]
    })
  </script>
  
  <style lang="scss" scoped></style>