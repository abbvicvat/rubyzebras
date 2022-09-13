<template>
    <div class="bg-green-500 w-full  pt-8">
      <center>
        <div class="w-1/6 text-xl rounded-full bg-red-400 hover:bg-yellow-500">
          <nuxt-link to="/About_Us">
            About Ruby Zebras
          </nuxt-link>
        </div>

        <div class="py-8">
          Copyright
          &copy;
          {{ year }}
          by Ruby Zebras, all rights reserved.
        </div>
      </center>
    </div>
</template>

<script>
export default {
  data () {
    return {
      year: new Date().getFullYear()
    }
  }
}
</script>
