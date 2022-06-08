<template>
    <div>
        <div class="container-jumbotron teachers-slider m-1">
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
            <div class="container mt-5">
                <h5 class="text-white text-center">Tüm Eğitmenler Gör</h5>
                <div class="slider-nav-button">
                    <span class="fa-solid fa-angle-left text-white left-arrow-1" @click="prevSlide"></span>
                    <span class="fa-solid fa-angle-left text-white left-arrow-2" @click="prevSlide"></span>
                    <span class="fa-solid fa-angle-left text-white left-arrow-3" @click="prevSlide"></span>
                    <span class="round-btn">
                        <span class="round-btn-2"></span>
                    </span>
                    <span class="fa-solid fa-angle-right text-white right-arrow-1" @click="nextSlide"></span>
                    <span class="fa-solid fa-angle-right text-white right-arrow-2" @click="nextSlide"></span>
                    <span class="fa-solid fa-angle-right text-white right-arrow-3" @click="nextSlide"></span>
                </div>
            </div>
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
                itemsToShow: 5,
                snapAlign: 'center',
                mouseDrag: false
            },
        }
    },
    methods: {
        nextSlide() {
            document.querySelector('.teachers-slider .carousel__next').click()
            console.log();
        },
        prevSlide() {
            document.querySelector('.teachers-slider .carousel__prev').click()
        }
    },
}
</script>

<style scoped>
.carousel__slide {
    margin: 10px;
    height: 320px;
    width: 230px !important;
    background-color: var(--theme-color-black);
    border-radius: 10px;
}

.carousel__item {
    position: relative;
    border-radius: 8px;
}

.carousel__item .slider-card-image {
    height: 320px;
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

.slider-nav-button {
    display: flex;
    justify-content: center;
    margin-top: 30px;
}

.slider-nav-button .round-btn {
    background-color: var(--theme-color-black);
    width: 45px;
    height: 45px;
    border-radius: 50%;
    border: 2px solid var(--theme-color-white);
    display: flex;
    justify-content: center;
    align-items: center;
}

.slider-nav-button .round-btn:hover {
    border: 3px solid #45A8EF;
    cursor: pointer;
}

.slider-nav-button .round-btn:hover .left-arrow-1 {
    background: #45A8EF !important;
}

.slider-nav-button .left-arrow-3:hover+.round-btn {
    border: 2px solid #45A8EF;
    cursor: pointer;
}

.slider-nav-button .left-arrow-3:hover {
    color: #45A8EF !important;
    cursor: pointer;
}

.slider-nav-button .left-arrow-2:hover {
    color: #45A8EF !important;
    cursor: pointer;
    opacity: 1;
}

.slider-nav-button .left-arrow-1:hover {
    color: #45A8EF !important;
    cursor: pointer;
    opacity: 1;
}

.slider-nav-button .right-arrow-2:hover {
    color: #45A8EF !important;
    cursor: pointer;
    opacity: 1;
}

.slider-nav-button .right-arrow-1:hover {
    color: #45A8EF !important;
    cursor: pointer;
    opacity: 1;
}

.slider-nav-button .right-arrow-3:hover {
    color: #45A8EF !important;
    cursor: pointer;
    opacity: 1;
}

.slider-nav-button .round-btn:hover .round-btn-2 {
    border: 2px solid #45A8EF;
    cursor: pointer;
}

.slider-nav-button .round-btn-2 {
    background-color: var(--theme-color-red);
    width: 2px;
    height: 2px;
    border-radius: 50%;
    border: 2px solid var(--theme-color-white);
}

.slider-nav-button .left-arrow-3,
.right-arrow-1 {
    margin-top: 10px;
    font-size: 25px;
}

.slider-nav-button .left-arrow-2,
.right-arrow-2 {
    margin-top: 13px;
    font-size: 20px;
    opacity: 0.5
}

.slider-nav-button .left-arrow-1,
.right-arrow-3 {
    margin-top: 15px;
    font-size: 15px;
    opacity: 0.3
}
</style>

