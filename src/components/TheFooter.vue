<template>
    <footer>
        <div class="container py-4">
            <div class="row py-2">
                <div class="col-5">
                    <div class="row text-white">
                        <div class="col">
                            <div class="d-flex flex-column">
                                <div>
                                    <h5 class="text-uppercase">Dc comics</h5>
                                    <ul class="list-unstyled">
                                        <li v-for="(link,id) in DcComicsLinks" :key="id">
                                            <a class="text-decoration-none text-capitalize" :href="link.href">{{link.name}}</a>
                                        </li>
                                    </ul>
                                </div>
                                <div>
                                    <h5 class="text-uppercase">shop</h5>
                                    <ul class="list-unstyled">
                                        <li v-for="(link,id) in shopLinks" :key="id">
                                            <a class="text-decoration-none text-capitalize" :href="link.href">{{link.name}}</a>
                                        </li>
                                    </ul>                                   
                                </div>
                            </div>
                        </div>
                        <div class="col">
                            <h5 class="text-uppercase">Dc</h5>
                                <ul class="list-unstyled">
                                        <li v-for="(link,id) in DcLinks" :key="id">
                                            <a class="text-decoration-none text-capitalize" :href="link.href">{{link.name}}</a>
                                        </li>
                                </ul> 
                        </div>
                        <div class="col">
                            <h5 class="text-uppercase">sites</h5>
                                <ul class="list-unstyled">
                                        <li v-for="(link,id) in sitesLinks" :key="id">
                                            <a class="text-decoration-none text-capitalize" :href="link.href">{{link.name}}</a>
                                        </li>
                                </ul> 
                        </div>
                    </div>
                </div>
                <div class="col">
                    <img src="/img/dc-logo-bg.png" alt="" class="bg-logo">
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
name: 'TheFooter',
data() {
    return {
        DcComicsLinks: [
            {
                name: 'characters',
                href: '#',
            },
            {
                name: 'comics',
                href: '#',
            },
            {
                name: 'movies',
                href: '#',
            },
            {
                name: 'tv',
                href: '#',
            },
            {
                name: 'games',
                href: '#',
            },
            {
                name: 'videos',
                href: '#',
            },
            {
                name: 'news',
                href: '#',
            }
        ],

        shopLinks: [
            {
                name: 'Shop DC',
                href: '#',
            },
            {
                name: 'Shop DC collectibles',
                href: '#',
            }
        ],

        DcLinks: [
            {
                name: 'term of Use',
                href: '#',
            },
            {
                name: 'privacy policy(New)',
                href: '#',
            },
            {
                name: 'ad choices',
                href: '#',
            },
            {
                name: 'advertising',
                href: '#',
            },
            {
                name: 'jobs',
                href: '#',
            },
            {
                name: 'subscription',
                href: '#',
            },
            {
                name: 'talent whorkshops',
                href: '#',
            },
            {
                name: 'CPSC certtificates',
                href: '#',
            },
            {
                name: 'ratings',
                href: '#',
            },
            {
                name: 'shop help',
                href: '#',
            },
            {
                name: 'contact us',
                href: '#',
            },
        ],

        sitesLinks: [
            {
                name: 'DC',
                href: '#',
            },
            {
                name: 'MAD magazine',
                href: '#',
            },
            {
                name: 'DC kids',
                href: '#',
            },
            {
                name: 'DC universe',
                href: '#',
            },
            {
                name: 'DC power visa',
                href: '#',
            },
        ]
    };
},
};
</script>

<style lang="scss">
@import "../assets/scss/main.scss";

    footer {
        background-image: url("../../public/img/footer-bg.jpg");
        background-size: cover;
        position: relative;
        z-index: 0;

        .bg-logo {
            position: absolute;
            right: 130px;
            top: -95px;
            z-index: -1;
        }

        a {
            font-size: 14px;
            color: grey;

            &:hover {
                color: $first;
            }
        }
    }
    
</style>