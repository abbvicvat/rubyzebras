<template>
    <div>
        <center>
            <img src="../static/images/zeebra.png" alt="">
            <div class="py-4 w-96">
                <div class="text-center text-green-500 text-4xl">Ruby Zebras</div>
                <div class="text-center text-yellow-500 text-2xl">Ruby Zebras</div>
                <div class="text-center">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                    incididunt ut labore
                    et dolore magna
                    aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
                    commodo
                    consequat. Duis
                    aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                    Excepteur sint
                    occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </div>
                <div class="flex justify-evenly mt-4">
                    <img src="../static/images/icons8-heart-48.png" alt="">
                    <img src="../static/images/icons8-add-shopping-cart-48.png" alt="">
                </div>
            </div>
        </center>
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

</style>