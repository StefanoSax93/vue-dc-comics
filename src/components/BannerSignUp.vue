<template>
    <div class="bg-banner py-4">
        <div class="container d-flex align-items-center justify-content-between">
            <a class="myButton text-uppercase">sign-up now</a>
            <div class="d-flex gap-3">
                <div class="fs-5">follow us</div>
                <img src="/img/footer-facebook.png" alt="">
                <img src="/img/footer-twitter.png" alt="">
                <img src="/img/footer-youtube.png" alt="">
                <img src="/img/footer-pinterest.png" alt="">
                <img src="/img/footer-periscope.png" alt="">
            </div>
        </div> 
    </div>
</template>

<script>
export default {
name: 'BannerSignUp',
};
</script>

<style lang="scss">
    @import "../assets/scss/main.scss";

    .bg-banner {
        background-color: $third;

        .fs-5 {
            color: $first;
            text-transform: uppercase;
            font-weight: bold;
        }
    }
    
</style>