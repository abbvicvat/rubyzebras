<template>
  <div>
    <div>
      Library
    </div>

    <div>
      <img :src="books[0].img"/>
      {{ books[0].title }}
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
