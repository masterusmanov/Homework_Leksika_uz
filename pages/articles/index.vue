<template>
    <div class="bg-green-50 pt-5">
        <main class="container min-h-screen mx-auto">
            <div class="flex">
                <div class="flex justify-beetwen items-center w-[70%] mt-5">
                    <div>
                        <div class="w-[100%] h-[74px] relative rounded-full bg-white flex justify-beetwen items-start">
                            <nuxt-link to="#"><i class='bx bx-search-alt-2 relative p-6 text-3xl text-gray-500 text-center'></i></nuxt-link>
                            <input type="text" placeholder="Search words here..." class="w-[74%] pl-5 relative text-xl h-[74px] rounded-full">
                        </div>
                        <Card/>
                        <Pagenation/>
                    </div>
                </div>
                <Something/>
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