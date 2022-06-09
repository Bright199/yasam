<template>
    <div class="container-jumbtron">
        <div class="container big-slider">
            <carousel :settings="settings">
                <slide v-for="image in imgUrl" :key="image.id">
                    <div class="carousel__item ">
                        <div class="row overlay">
                            <div class="col-md-2"></div>
                            <div class="col-md-6 overlay-content">
                                <p class="text-white">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil, explicabo sed,
                                    consequatur cupiditate error quod obcaecati soluta voluptates ipsam hic debitis
                                    cumque quasi fugit quaerat, temporibus quas doloribus distinctio nobis?</p>
                                    <h4 class="text-white">Mr Dolor Sir</h4>
                                    <p class="text-white">CEO</p>
                            </div>
                            <div class="col-md-2"></div>
                        </div>
                        <div class="row py-4">
                            <div class="col-md-1"></div>
                            <div class="col-md-5 main-text-container">
                                <h2 class="text-white">Hakkımızda</h2>
                                <h3 class="text-white">Ne söylediler?</h3>
                                <div class="left-bar"></div>
                            </div>
                            <div class="col-md-5 p-0">
                                <div class="slider-image">
                                    <img src="@/assets/images/skyscrapper.png" alt="">
                                </div>
                            </div>
                            <div class="col-md-1"></div>
                        </div>
                    </div>
                </slide>

                <template #addons>
                    <navigation />
                    <pagination />
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

<style >
.big-slider .carousel__item{
    position: relative;
}
.big-slider .carousel__item .slider-image {
    height: 500px;
    width: 100%;
}

.big-slider .carousel__item .slider-image img {
    height: 100%;
    width: 100%;
    border-radius: 10px;
}

.big-slider .carousel__pagination-button {
    margin: var(--vc-pgn-margin);
    width: 10px;
    height: 10px;
    border-radius: 50%;
    border: 1px solid var(--theme-color-white);
    cursor: pointer;
    background-color: var(--theme-color-black) !important;
}

.big-slider .carousel__pagination-button--active {
    background-color: var(--theme-color-white) !important;
}

.main-text-container {
    padding-top: 65px;
    position: relative;
}

.main-text-container .left-bar {
    background-color: #B678FF;
    width: 4px;
    height: 70px;
    top: 70px;
    left: 120px;
    position: absolute;
    border-radius: 10px;

}

.big-slider .carousel__item .overlay{
    position: absolute;
    bottom: 60px;
}
.big-slider .carousel__item .overlay .overlay-content{
    text-align:start;
    background-color:#1E1E1E;
    padding: 25px;
    border-radius: 10px;
}

.big-slider .carousel__prev--in-active,.carousel__next--in-active {
    display: block !important;
}
</style>

