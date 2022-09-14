<template>
  <div>
    <div class="text text-green-500">
      Library
    </div>

    <div class="flex justify-evenly flex-wrap">
      <div class="mt-12">
        <img class="w-96" :src="books[0].img" />
        <div class="text-center">{{ books[0].title }}</div>
      </div>

      <div class="mt-12">
        <img class="w-96" :src="books[1].img" />
        <div class="text-center">{{books[1].title}}</div>
      </div>

      <div>
        <div class="mt-12">
          <img class="w-96" :src="books[2].img" />
          <div class="text-center">{{ books[2].title}}</div>
        </div>
      </div>

      <div>
        <div class="mt-12">
          <img class="w-96" :src="books[4].img" />
          <div class="text-center">{{ books[4].title}}</div>
        </div>
      </div>

      <div>
        <div class="mt-12">
          <img class="w-96" :src="books[3].img" />
          <div class="text-center">{{ books[3].title}}</div>
        </div>
      </div>

      <div>
        <div class="mt-12">
          <img class="w-96" :src="books[5].img" />
          <div class="text-center">{{ books[5].title}}</div>
        </div>
      </div>

      <div>
        <div class="mt-12">
          <img class="w-96" :src="books[6].img" />
          <div class="text-center">{{ books[6].title}}</div>
        </div>
      </div>

    </div>

  </div>
</template>

<script>
import data from '../db.json'
export default {
  async fetch () { this.books = data.books },
  data () {
    return {
      books: []
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

img:hover {
  transform: scale(1.05);
  transition-duration: 0.7s;
}
</style>
