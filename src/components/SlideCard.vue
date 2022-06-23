<template>
    <div>
        <div class="position-relative">
        <img :src="slideUrl" :alt="`Immagine di ${slideSeries}`" class="thumb d-block">
        <div class="slide-overlay p-3">
            <h6><strong>Prezzo:</strong> {{slidePrice}}</h6>
            <h6><strong>Tipo:</strong> {{slideType}}</h6>
        </div>
    </div>
    <h6 class="text-uppercase">{{slideSeries}}</h6>
    </div>
</template>

<script>
export default {
    props: {
        slideUrl: String,
        slideSeries: String,
        slidePrice: String,
        slideType: String
    }
}
</script>

<style lang="scss">
.thumb {
    width: 100%;
    aspect-ratio: 1/1;
    object-fit: cover;
    object-position: top;
    margin-bottom: 10px;
    transition: all .3s ease-in-out;
}
.slide-overlay {
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background-color: rgba(0,0,0,0.5);
        transition: all .3s ease-in-out;
        opacity: 0;

        &:hover {
            opacity: 1;
        }
    }

</style>