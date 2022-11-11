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
}
</style>

