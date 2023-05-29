<template>
    <div class="bg-green-50 pt-10">
        <main class="min-h-screen">
            <div class="mt-10">
                <BtnSearch titleq="RUS ⇆ UZB"/>
                <div class="mt-10">
                    <StartWord/>
                </div>
                <div class="mt-10">
                    <Search />
                </div>
                <div class="mt-10">
                    <ErrorRus/>
                </div>
            </div>
        </main>
    </div>
  </template>
  
  <script setup>
   const {name} = useRoute();
    useHead({
        title: `RUS ⇆ UZB page of Leksika.uz`,
        meta: [
        {
            name: "description", content: `RUS ⇆ UZB page of Leksika.uz`
        },
        {
            name: "author", content: "Leksika.uz"
        }
        ]
    })
  </script>
  
  <style lang="scss" scoped></style>