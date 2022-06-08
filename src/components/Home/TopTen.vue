<template>
    <div>
        <div class="container-jumbotron pupular-slider m-1">
            <div class=" row">
                <div class="col-md-1"></div>
                <div class="col-md-11  p-2">
                    <h5 class="text-white mb-5">Top 10 Eğitim Listesi</h5>
                    <carousel :settings="settings">
                        <slide v-for="image in imgUrl" :key="image.id" >
                            <div class="carousel__item " :class="image.live === 'yes' ? 'liveCard' : ''">
                                <div class="slider-card-image">
                                    <img :src="image.url" alt="scrapper">
                                </div>
                                <div class="slider-car-alt">
                                    <div class="row">
                                        <div class="col-md-7">
                                            <p class="text-white">{{ image.alt_text }}</p>
                                        </div>
                                        <div class="col-md-5"></div>
                                    </div>
                                </div>
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
import personBag from '@/assets/images/person_bag.png'
import skyScrapper from '@/assets/images/skyscrapper.png'
import person1 from '@/assets/images/person1.png'
import person2 from '@/assets/images/person2.png'
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
                { id: 1, url: skyScrapper, alt_text: 'Lorem ipsum dolor sit amet.', live: 'yes' },
                { id: 2, url: personBag, alt_text: 'Lorem ipsum dolor sit amet.', live: 'no' },
                { id: 3, url: person1, alt_text: 'Lorem ipsum dolor sit amet.', live: 'yes' },
                { id: 4, url: person2, alt_text: 'Lorem ipsum dolor sit amet.', live: 'no' },
                { id: 5, url: person1, alt_text: 'Lorem ipsum dolor sit amet.', live: 'no' },
                { id: 6, url: skyScrapper, alt_text: 'Lorem ipsum dolor sit amet.', live: 'no' },
                { id: 7, url: person2, alt_text: 'Lorem ipsum dolor sit amet.', live: 'no' },
                { id: 8, url: personBag, alt_text: 'Lorem ipsum dolor sit amet.', live: 'no' },
            ],
            settings: {
                itemsToShow: 5,
                snapAlign: 'center',
                // mouseDrag: false
            },
        }
    },
}
</script>

<style scoped>
.carousel__slide {
    margin: 10px;
    height: 150px;
    width: 200px;
    padding: 0;
    background-color: blue;
    border-radius: 10px;
}

.carousel__item {
    position: relative;
    border-radius: 8px;
}

.carousel__item .slider-card-image {
    height: 150px;
    width: 100%;
}

.carousel__slide img {
    width: 100%;
    height: 100%;
    border-radius: 10px
}

.carousel__slide .slider-car-alt {
    position: absolute;
    bottom: 0;
    background: linear-gradient(180deg, rgba(0, 0, 0, 0) 0%, #000000 100%);
}

.liveCard {
    border: .1px solid rgb(255, 44, 44)
}



</style>