<template>
    <div>
        <div class="container m-1">
            <carousel :settings="settings">
                <slide v-for="image in imgUrl" :key="image.id">
                    <div class="carousel__item ">
                        <div class="slider-card-image">
                            <img :src="image.url" alt="scrapper">
                        </div>
                    </div>
                </slide>

                <template #addons >
                    <navigation />
                </template>
            </carousel>
            
        </div>

    </div>
</template>

<script>
import blackface1 from '@/assets/images/blackface1.png'
import blackface2 from '@/assets/images/blackface2.png'
import blackface3 from '@/assets/images/blackface3.png'
import blackface4 from '@/assets/images/blackface4.png'
import blackface5 from '@/assets/images/blackface5.png'
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';
import 'vue3-carousel/dist/carousel.css';
export default {
    name: 'PopularEgitmler',
    components: {
        Carousel,
        Slide,
        Pagination,
        Navigation,
    },

    data() {
        return {
            imgUrl: [
                { id: 1, url: blackface2 },
                { id: 2, url: blackface4 },
                { id: 3, url: blackface3 },
                { id: 4, url: blackface5 },
                { id: 5, url: blackface2 },
                { id: 6, url: blackface4 },
                { id: 7, url: blackface3 },
                { id: 8, url: blackface2 }
            ],
            settings: {
                itemsToShow: 1,
                snapAlign: 'center',
                mouseDrag: false
            },
        }
    },
    methods: {
        // nextSlide() {
        //     document.querySelector('.teachers-slider .carousel__next').click()
        //     console.log();
        // },
        // prevSlide() {
        //     document.querySelector('.teachers-slider .carousel__prev').click()
        // }
    },
}
</script>

<style scoped>
.carousel__slide {
    
}

.carousel__item {
    
}

.carousel__item .slider-card-image {
    
}

.carousel__slide img {
    
}

.carousel__slide .slider-car-alt {
    
}



</style>

