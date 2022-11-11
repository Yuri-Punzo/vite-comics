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
    </div>
</template>

<style lang="scss" scoped>
#site_main {
    background-color: black;
    color: white;
    height: 200px;
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>

