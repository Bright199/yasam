<template>
    <div>
        <div class="container pupular-slider">
            <div class=" row">
                <div class="col-md-1"></div>
                <div class="col-md-11  p-2">
                    <h5 class="text-white mb-5">Big slider</h5>
                    <carousel :items-to-show="5" class="bg-light">
                        <slide v-for="slide in 10" :key="slide">
                            {{ slide }}
                        </slide>

                        <template #addons>
                            <navigation />
                            <pagination/>
                        </template>
                    </carousel>
                </div>
            </div>
        </div>

    </div>
</template>

<script>
import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';
export default {
    name: 'TopTen',
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