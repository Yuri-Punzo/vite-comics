<script>
import Products from "./Products.vue"

export default {
    name: "SiteMain",
    components: {
        Products
    }
}
</script>

<template>
    <div id="site_main">
        <div class="position-relative">
            <span class="curremt_series_tag">CURRENT SERIES</span>
        </div>

        <Products />

        <div class="text-center py-4">
            <span class="load_more_btn">LOAD MORE</span>
        </div>
    </div>
</template>

<style lang="scss" scoped>
#site_main {
    background-color: black;
    color: white;
}

.load_more_btn {
    background-color: #0282f9;
    padding: 0.5rem 2.5rem;
    font-weight: bold;

    &:hover {
        cursor: pointer;
    }
}

.curremt_series_tag {
    background-color: #0282f9;
    padding: 0 1rem;
    font-weight: bold;
    font-size: 25px;
    position: absolute;
    top: -18px;
    left: 160px;
}
</style>

