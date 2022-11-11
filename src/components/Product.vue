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
    <div class="col">
        <div>
            <img :src="image" :alt="title">
            <h5 class="py-2">{{ title }}</h5>
        </div>
    </div>
</template>

<style lang="scss" scoped>
img {
    height: 185px;
    aspect-ratio: 1 / 1;
    object-fit: cover;
    object-position: top;
}
</style>