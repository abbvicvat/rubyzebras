
<template>
  <div class="h-screen">
    <Header />
    <nuxt class="min-h-full" />
    <Footer />
  </div>
</template>

<script>
export default {
  head () {
    return {
      title: "Ruby Zebras"
    }
  },
}
</script>
