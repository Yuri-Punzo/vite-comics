<script>
export default {
    name: "SiteFooterBottom"
}
</script>

<template>
    <div id="site_footer_bottom">
        <div class="container">
            <div class="row">
                <div class="col my_col">
                    <span class="my_button">SIGN-UP NOW!</span>
                </div>
                <div class="col my_col_end">
                    <span class="follow_us">FOLLOW US</span>
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">

                </div>
            </div>

        </div>
    </div>
</template>

<style lang="scss" scoped>
#site_footer_bottom {
    background-color: #303030;
    font-size: 14px;
}

.my_button {
    padding: 0.5rem 1rem;
    border: 2px solid #0282fa;
    color: white;
}

.my_col {
    display: flex;
    align-items: center;
}

.my_col_end {
    display: flex;
    justify-content: flex-end;
    align-items: center;

    img {
        padding: 1rem 0.5rem;
    }
}

.follow_us {
    color: #0282fa;
    font-weight: bold;
}
</style>