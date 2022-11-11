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
</style>

