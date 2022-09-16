<template>
  <div>
    <!--"npm run start-server" -->
    <div>
      <carousel :slides="slides" :interval="5000" controls indicators />
    </div>
    <hr class="mt-16">

    <div class="flex justify-center m-16 text-green-500 text-2xl">
      Top rated book
    </div>
    <nuxt-link to="/Books">
      <div class="flex flex-wrap">
        <div class="w-1/2">
          <img class="shadow-xl ml-24 w-5/6" src="../static/images/zeebra.png">
        </div>
        <div class="flex items-center text-4xl ml-16 w-1/3">
          Den här boken handlar om undervattens zebror som lever i corallrev
        </div>
      </div>
    </nuxt-link>
    <hr class="mt-16">

    <div class="flex justify-center m-16 text-green-500 text-2xl">
      Most viewed
    </div>
    <div class="flex flex-wrap">
      <div class="flex items-center text-4xl ml-16 w-1/3">
        Det här är historian om den sällsynta pickfågeln som bara flyger 5 gånger per år.
      </div>
      <div class="w-1/2">
        <img class="shadow-xl ml-24 w-5/6" src="../static/images/bird.jpg" alt="">
      </div>
    </div>
    <hr class="mt-16">

    <div class="flex justify-center m-16 text-green-500 text-2xl">
      Habitats
    </div>
    <div class="flex flex-wrap m-32 justify-center">
      <NuxtLink to="/Library" class="w-2/5">
        <img src="https://cdn-icons-png.flaticon.com/512/6619/6619693.png" alt="">
      </NuxtLink>
      <NuxtLink to="/Library" class="w-2/5">
        <img src="https://cdn-icons-png.flaticon.com/512/414/414825.png" alt="">
      </NuxtLink>
      <NuxtLink to="/Library" class="mt-8 w-2/5">
        <img src="https://cdn-icons-png.flaticon.com/512/3254/3254422.png" alt="">
      </NuxtLink>
      <NuxtLink to="/Library" class="mt-8 w-2/5">
        <img src="https://cdn-icons-png.flaticon.com/512/3038/3038873.png" alt="">
      </NuxtLink>
    </div>
  </div>
</template>

<script>
import Header from "../components/Header.vue"
export default {
  name: "IndexPage",
  data: () => ({
    slides: [
      "https://picsum.photos/id/1032/900/400",
      "https://picsum.photos/id/1033/900/400",
      "https://picsum.photos/id/1037/900/400",
      "https://picsum.photos/id/1035/900/400",
      "https://picsum.photos/id/1036/900/400",
    ],
  }),
}
</script>
