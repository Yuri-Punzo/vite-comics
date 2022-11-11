<script>
import Product from "./Product.vue"
import products from "../data/dc-comics.js"

export default {
    name: "Products",
    components: {
        Product
    },
    data() {
        return {
            comics: products
        }
    }
}
</script>

<template>
    <div class="container pt-5">
        <div class="row g-2">
            <Product v-for="comic in comics" :image="comic.thumb" :title="comic.series.toUpperCase()" />
        </div>
    </div>

</template>

<style lang="scss" scoped>

</style>