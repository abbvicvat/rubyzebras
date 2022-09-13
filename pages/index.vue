<template>
  <div>
    <div class="flex justify-center m-16">
      Top rated book
    </div>
  <div class="flex flex-wrap">
    <div class="w-1/2">
      <img class="shadow-xl ml-24" src="../static/images/zeebra.png">
    </div>
    <div class="flex items-center text-4xl ml-16 w-1/3">
        Den här boken handlar om undervattens zebror som lever i corallrev
    </div>
  </div>
  <hr class="mt-16">

  <div class="flex justify-center m-8">
    most viewed
  </div>
<center>
  <div class="flex justify-center w-1/2">
    <img class="" src="../static/images/bird.jpg" alt="">
  </div>
  <div class="m-16 text-2xl w-1/2">
    Det här är historian om den sällsynta pickfågeln som bara flyger 5 gånger per år.
  </div>
</center>

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
}
</script>
