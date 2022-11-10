<script>
export default {
    name: "SiteFooterTop"
}
</script>

<template>
    <div id="site_footer_top">
        <div class="container">
            <div class="row">
                <div class="col">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                    <span>DIGITAL COMICS</span>
                </div>
                <div class="col">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    <span>DC MERCHANDISE</span>
                </div>
                <div class="col">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    <span>SUBSCRIPTION</span>
                </div>
                <div class="col">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    <span>COMIC SHOP LOCATOR</span>
                </div>
                <div class="col">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    <span>DC POWER VISA</span>
                </div>
            </div>
        </div>
    </div>

</template>

<style lang="scss" scoped>
#site_footer_top {
    background-color: #0282f9;
    color: white;
    font-size: 12px;
}

.col {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 1.5rem;

    img {
        height: 55px;
        padding: 0.5rem;
    }

    &:hover {
        cursor: pointer;
    }
}
</style>