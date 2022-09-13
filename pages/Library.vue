<template>
  <div>
    <div>
      Library
    </div>



    <div class="flex-wrap">
      <img class="w-96" :src="books[0].img"/>
      <div class="">{{ books[0].title }}</div>
    </div>

    <div class="flex-wrap">
      <img class="w-96" :src="books[1].img"/>
      <div class="">{{books[1].title}}</div>

    </div>

  </div>
</template>

<script>
export default {
  data() {
    return {
      books: []
    }
  },
  async fetch () {
  this.books = await fetch(
    "http://localhost:5000/books"
    ).then(res => res.json())
  }
}
</script>

<style>
</style>
