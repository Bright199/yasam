<template>
    <div>
        <div class="container-jumbotron pupular-slider">
            <carousel :items-to-show="5" class="bg-light">
                <slide v-for="slide in 10" :key="slide">
                    {{ slide }}
                </slide>

                <template #addons>
                    <navigation />
                </template>
            </carousel>
            <div class="container">
                <h5 class="text-white">Tüm Eğitmenler Gör</h5>
                <span class="fa-solid fa-angle-left text-white"></span>
                <button class="round-btn">Round</button>
                <span class="fa-solid fa-angle-right text-white"></span>
            </div>
        </div>

    </div>
</template>

<script>
import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';
export default {
    name: 'AllTeachers',
    components: {
        Carousel,
        Slide,
        Pagination,
        Navigation,
    },
}
</script>

<style>
</style>