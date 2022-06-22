<template>
<div>
    <div class="container d-flex justify-content-between align-items-center py-3">
        <img src="/img/dc-logo.png" alt="">
        <ul class="nav">
            <li class="nav-item" v-for="(link,id) in navLinks" :key="id">
                <a class="nav-link text-uppercase text-dark fw-bold" aria-current="page" :href="link.href">{{link.name}}</a>
                <div class="hover-bar"></div>
            </li>
        </ul>
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
@import "../assets/scss/variables.scss";
.nav-item {
    border-bottom: 3px solid transparent;
    font-size: 13px;

    
    .hover-bar {
        height: 5px;
        background-color: $first;
        opacity: 0;
        transition: all .3s ease-in-out;
        position: relative;
        top: 49px;
    }

    &:hover .hover-bar {
            opacity: 1;
        }
}

.bg-second {
    background-color: $second;
}

</style>