<script>
import products from "./data/dc-comics.js"
import Product from "./Product.vue"

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
    <div class="container">
        <div class="row">
            <Product v-for="comic in comics" :image="Product.src" :title="Product.title" />
        </div>
    </div>
</template>

<style lang="scss" scoped>

</style>