<template>
  <div>
    <div class="text text-green-500">
      Library
    </div>
    <div class="flex justify-evenly flex-wrap">
      <template v-for="book in books">
        <div class="mt-12 mx-96 w-full flex flex-wrap justify-center" v-if="book.img != null" :key="book.id">
          <div class="flex flex-wrap cont">
            <img class="w-72" :src="book.img" />
            <div class="pl-8 w-80">
              <div class="text-center text-green-500 text-2xl">{{ book.title }}</div>
              <div class="text-center text-yellow-500 text-lg">{{ book.author }}</div>
              <div class="text-center">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                incididunt ut labore
                et dolore magna
                aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
                consequat. Duis
                aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                Excepteur sint
                occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</div>
              <div class="flex justify-evenly mt-4">
                <img src="../static/images/icons8-heart-48.png" alt="">
                <img src="../static/images/icons8-add-shopping-cart-48.png" alt="">
              </div>
            </div>
          </div>
        </div>
      </template>
    </div>
  </div>
</template>

<script>
import data from '../db.json'
export default {
  data () {
    return {
      books: data.books
    }
  }
}
</script>

<style>
.text {
  display: flex;
  font-size: 50px;
  justify-content: center;

}

.cont:hover {
  transform: scale(1.05);
  transition-duration: 0.7s;
}
</style>
