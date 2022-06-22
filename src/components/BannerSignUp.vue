<template>
    <div class="bg-banner py-4">
        <div class="container d-flex align-items-center justify-content-between">
            <a class="myButton text-uppercase" href="#">sign-up now</a>
            <div class="d-flex gap-3">
                <div class="fs-5">follow us</div>
                <a v-for="(social,id) in socialList" :key="id" :href="social.href">
                    <img :src="social.img" :alt="social.alt">
                </a>
            </div>
        </div> 
    </div>
</template>

<script>
export default {
name: 'BannerSignUp',
data() {
    return {
        socialList: [
            {
                img: '/img/footer-facebook.png',
                href: '#',
                alt: 'facebook'
            },
            {
                img: '/img/footer-twitter.png',
                href: '#',
                alt: 'twitter'
            },
            {
                img: '/img/footer-youtube.png',
                href: '#',
                alt: 'youtube'
            },
            {
                img: '/img/footer-pinterest.png',
                href: '#',
                alt: 'pinterest'
            },
            {
                img: '/img/footer-periscope.png',
                href: '#',
                alt: 'periscope'
            },
        ]
    }
}
};
</script>

<style lang="scss">
    @import "../assets/scss/variables.scss";

    .bg-banner {
        background-color: $third;
        position: relative;
        z-index: 0;

        .fs-5 {
            color: $first;
            text-transform: uppercase;
            font-weight: bold;
        }

        a:hover {
            transform: scale(1.2);
            transition: transform .3s ease-in-out;
        }
    }
    
</style>