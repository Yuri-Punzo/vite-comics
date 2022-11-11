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
        <div class="text-center py-4">
            <span class="load_more_btn">LOAD MORE</span>
        </div>
    </div>

</template>

<style lang="scss" scoped>
.load_more_btn {
    background-color: #0282f9;
    padding: 0.5rem 2.5rem;
    font-weight: bold;

    &:hover {
        cursor: pointer;
    }
}
</style>