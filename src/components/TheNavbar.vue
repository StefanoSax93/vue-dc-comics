<template>
<div>
    <div class="container d-flex justify-content-between align-items-center py-3">
        <img src="/img/dc-logo.png" alt="">
        <ul class="nav">
            <li class="nav-item" v-for="(link,id) in navLinks" :key="id">
                <a class="nav-link text-uppercase text-dark fw-bold" aria-current="page" :href="link.href">{{link.name}}</a>
            </li>
        </ul>
    </div>
    <div class="bg-dark py-5 text-white">
        <div class="container">
            --> Content Goes Here --
        </div>
    </div>
</div>
</template>



<script>
export default {
name: 'TheNavbar',
data() {
    return {
        navLinks: [
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
                name: 'collectibles',
                href: '#',
            },
            {
                name: 'videos',
                href: '#',
            },
            {
                name: 'fans',
                href: '#',
            },
            {
                name: 'news',
                href: '#',
            },
            {
                name: 'shop',
                href: '#',
            },
        ],
    }
},
};
</script>

<style lang="scss">
@import "../assets/scss/main.scss";
.nav-item {
    border-bottom: 3px solid transparent;
    font-size: 13px;

    &:hover {
        border-bottom: 3px solid $primary;
    }
}

</style>