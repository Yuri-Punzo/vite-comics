<script>
export default {
    name: "SiteFooterCenter"
}
</script>

<template>
    <div id="site_footer_center">
        <div class="container">
            <div class="row">
                <div class="col-auto my_col">
                    <h2>DC COMICS</h2>
                    <a href="">Characters</a>
                    <a href="">Comics</a>
                    <a href="">Movies</a>
                    <a href="">TV</a>
                    <a href="">Games</a>
                    <a href="">Videos</a>
                    <a href="">News</a>
                    <h2>SHOP</h2>
                    <a href="">Shop DC</a>
                    <a href="">Shop DC Collectibles</a>
                </div>
                <div class="col-auto my_col">
                    <h2>DC</h2>
                    <a href="">Term Of Use</a>
                    <a href="">Privacy Policy(New)</a>
                    <a href="">Ad Choices</a>
                    <a href="">Advertising</a>
                    <a href="">Jobs</a>
                    <a href="">Subscriptions</a>
                    <a href="">Talent Workshops</a>
                    <a href="">CPSC Certificates</a>
                    <a href="">Ratings</a>
                    <a href="">Shop Help</a>
                    <a href="">Contact Us</a>
                </div>
                <div class="col-auto my_col">
                    <h2>SITES</h2>
                    <a href="">DC</a>
                    <a href="">MAD Magazine</a>
                    <a href="">DC Kids</a>
                    <a href="">DC Universe</a>
                    <a href="">DC Power Visa</a>
                </div>
                <div class="col col_dc_bg">

                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
#site_footer_center {
    background-image: url(../assets/img/footer-bg.jpg);
}

.my_col {
    padding: 2rem 1rem;

    h2 {
        color: white;
    }

    a {
        color: gray;
        font-size: 8;
        display: block;
        text-decoration: none;

        &:hover {
            color: #0282f9;
        }
    }
}

.col_dc_bg {
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: right;
}
</style>