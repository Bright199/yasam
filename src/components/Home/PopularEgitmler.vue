<template>
    <div>
        <div class="container-jumbotron pupular-slider">
            <div class=" row">
                <div class="col-md-1"></div>
                <div class="col-md-11  p-2">
                    <h5 class="text-white mb-5">Popülar Eğitmler</h5>
                    <carousel :items-to-show="5" >
                        <slide v-for="slide in 10" :key="slide">
                            <div class="live-card slider-card">
                                {{ slide }}
                            </div>
                        </slide>

                        <template #addons>
                            <navigation />
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
    name: 'PopularEgitmler',
    components: {
        Carousel,
        Slide,
        Pagination,
        Navigation,
    },
}
</script>

<style scoped>
.live-card {
    width: 250px;
    height: 150px;
    border-radius: 8px;
    margin: 10px;
    background-color: var(--theme-color-blue);
}
</style>