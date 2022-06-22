<template>
    <div>
        <img :src="slideUrl" :alt="`Immagine di ${slideSeries}`" class="thumb">
        <h6 class="text-uppercase">{{slideSeries}}</h6>
    </div>
</template>

<script>
export default {
    props: {
        slideUrl: String,
        slideSeries: String,
    }
}
</script>