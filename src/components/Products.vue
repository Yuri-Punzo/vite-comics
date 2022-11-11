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
        <div class="position-relative">
            <span class="curremt_series_tag">CURRENT SERIES</span>
        </div>
        <div class="row row-cols-sm-2 row-cols-md-3 row-cols-lg-4 row-cols-xxl-6 g-2">
            <Product v-for="comic in comics" :image="comic.thumb" :title="comic.series.toUpperCase()" />
        </div>

    </div>

</template>

<style lang="scss" scoped>
.curremt_series_tag {
    background-color: #0282f9;
    padding: 0 1rem;
    font-weight: bold;
    font-size: 25px;
    position: absolute;
    top: -67px;
    left: -12px;
}
</style>