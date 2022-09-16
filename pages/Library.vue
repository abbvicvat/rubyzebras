<template>
  <div>
    <div class="text text-green-500">
      Library
    </div>

    <div class="flex justify-evenly flex-wrap">


      <template v-for="book in books">
        <div class="mt-12 mx-96 w-full border flex flex-wrap justify-center" v-if="book.img != null" :key="book.id">
          <div class="flex flex-wrap">
            <img class="w-72" :src="book.img" />
            <div class="w-40">
              <div class="text-center">{{ book.title }}</div>
              <div class="text-center">{{ book.author }}</div>
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
  },
  // async fetch () {
  //   this.books = await fetch(
  //     "http://localhost:5000/books"
  //   ).then(res => res.json())
  // }

}
</script>

<style>
.text {
  display: flex;
  font-size: 50px;
  justify-content: center;

}

/* 
img :hover {
  transform: scale(1.05);
  transition-duration: 0.7s;
} */
</style>
