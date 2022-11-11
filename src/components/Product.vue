<script>
export default {
    name: "Product",
    props: {
        image: String,
        title: String
    }
}
</script>

<template>
    <div class="col-2">
        <img :src="image" alt="">
        <p>{{ title }}</p>
    </div>
</template>

<style lang="scss" scoped>

</style>