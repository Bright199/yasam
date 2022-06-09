<template>
    <div class=" position-relative p-0">
        <div class="small-screen-nav">
            <SmallNav/>
        </div>
        <nav class="container large-screen-nav">
            <ul class="left-nav">
                <li class="logo-link">
                    <router-link to="/">
                        <img src="../../assets/images/logo.png" alt="logo-image">
                        <span class="yasam-text">yaşam</span> atölyesi
                    </router-link>
                </li>
                <li>
                    <router-link to="/" class="anasayfa-link">
                        Anasayfa
                    </router-link>
                </li>
                <li>
                    <router-link to="#">
                        Kategoriler
                    </router-link>
                </li>
                <li>
                    <router-link to="#">
                        <span class="atolye-text">Atölye</span> <span class="plus-sign">+</span>
                    </router-link>
                </li>
                <li>
                    <router-link to="#">
                        Eğitmenlerimiz
                    </router-link>
                </li>
                <li>
                    <router-link to="#">
                        Planlar
                    </router-link>
                </li>
                <li>
                    <router-link to="#" class="kesfet-btn">
                        Keşfet
                    </router-link>
                </li>
            </ul>

            <ul class="right-nav">
                <li>
                    <router-link to="#">
                        <i class="fa-solid fa-magnifying-glass"></i>
                    </router-link>
                </li>
                <li>
                    <router-link to="#" class="login-btn">
                        Giriş Yap
                    </router-link>
                </li>
            </ul>
        </nav>

        <div class="container-jumbotron coughing-container ">
            <div class="container pt-5 ">
                <div class="row p-0">
                    <div class="col-md-6 mt-4 ">
                        <h2>Business</h2>
                        <h2>Coaching</h2>
                        <p>Lorem ipsum dolor adipisicing elit. Eveniet fuga nesciunt delectus
                            natus. Nam magnam dolores qui facere esse ut nemo debitis laborum. Est repellendus dolores
                            quaerat esse tenetur alias?</p>
                        <button class="abone-ol">Abone Ol</button>
                    </div>
                </div>
            </div>
        </div>
        <div class="colors">
            <div class="blur-1 blur"></div>
            <div class="blur-2 blur"></div>
            <div class="blur-3 blur"></div>
        </div>
        <div class="manifesto">
            <div class="container p-4 ">

                <div class="row">
                    <div class="col-md-1"></div>
                    <div class="col-md-2 manifesto-text">
                        <p class="yasam-atolye">Yaşam Atölyesi</p>
                        <h3>Manifesto</h3>
                        <div>
                        </div>

                    </div>
                    <div class="col-md-8 manifesto-long-text">
                        <blockquote id="manifesto-quote">
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo, dicta rerum. Qui,
                                commodi
                                impedit distinctio fuga itaque accusamus voluptatum deleniti molestias architecto, eos
                                sit
                                reiciendis repellendus! Cumque quas id in. Lorem ipsum dolor sit amet consectetur
                                adipisicing elit.</p>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo, dicta rerum. Qui,
                                commodi
                                impedit distinctio fuga itaque accusamus voluptatum deleniti molestias architecto, eos
                                sit
                                reiciendis repellendus! Cumque quas id in. Lorem ipsum, dolor sit amet consectetur
                                adipisicing elit.</p>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo, dicta rerum. Qui,
                                commodi
                                impedit distinctio fuga itaque accusamus voluptatum deleniti molestias architecto, eos
                                sit
                                reiciendis repellendus! Cumque quas id in. Lorem, ipsum dolor sit amet consectetur
                                adipisicing elit.</p>
                        </blockquote>
                    </div>
                    <div class="col-md-1"></div>
                </div>
            </div>
        </div>

        <div>
            <PopularEgitmler />
        </div>

        <div class="container-jumbotron kesfet-container ">
            <div class="container pt-5 ">
                <div class="row p-0">
                    <div class="col-md-6 mt-4 ">
                        <h2>Keşfet</h2>
                        <p>Lorem ipsum dolor adipisicing elit. Eveniet fuga nesciunt delectus
                            natus. Nam magnam dolores qui facere esse ut nemo debitis laborum. Est repellendus dolores
                            quaerat esse tenetur alias?</p>
                        <button class="kesfet-btn">Keşfete Git</button>
                    </div>
                </div>
            </div>
        </div>

        <div>
            <TopTen />
        </div>

        <div class="colors-2">
            <div class="blur-1-2 blur"></div>
            <div class="blur-2-2 blur"></div>
            <div class="blur-3-2 blur"></div>
        </div>

        <div class="odeme-planlar">
            <div class="container">
                <div class="row">
                    <div class="col-md-3"></div>
                    <div class="col-md-6">
                        <h2 class="text-white text-center">Ödeme Planları</h2>
                        <p class="text-center text-white">Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                            Dolore,
                            accusantium repudiandae aliquid
                            doloremque ut vero quia nobis nisi tempore molestias earum, eligendi cum labore officia
                            voluptates
                            exercitationem, ipsa nesciunt quod.</p>
                    </div>
                    <div class="col-md-3"></div>
                </div>

                <div class="odeme-card">
                    <div class="aylik-plan aylik-plan-1">
                        <p>Aylik plan</p>
                        <h4>90TL</h4>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing.</p>
                        <button class="aylik-plan-btn">Plan Seç</button>
                    </div>
                    <div class="aylik-plan aylik-plan-2">
                        <p>Aylik plan</p>
                        <h4>890TL</h4>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing.</p>
                        <button class="aylik-plan-btn">Plan Seç</button>
                    </div>
                    <div class="aylik-plan aylik-plan-3">
                        <p>Aylik plan</p>
                        <h4><span class="atoly-plan-text">Atölye</span> <span class="plan-plus-sign">+</span></h4>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing.</p>
                        <button class="aylik-plan-btn">Detaylı Bilgi</button>
                    </div>
                </div>

                <div class="nasil-calisir mt-5">
                    <div class="container">
                        <div class="row">
                            <div class="col-md-6 nasil-text-container">
                                <h2 class="text-white">Nasıl Çalışır?</h2>
                                <p class="text-white">Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                                    Repudiandae totam
                                    consequatur quo neque omnis. Quam iure vitae.</p>
                                <div class="pink-divider"></div>

                                <q class="text-white">
                                    Lorem ipsum dolor sit, amet consectetur adipisicing elit. Numquam, autem iusto
                                    inventore, quod similique excepturi impedit itaque porro, repellendus quo odio
                                    quaerat aspernatur ea cum unde amet. Unde, autem repudiandae?
                                </q>
                            </div>
                            <div class="col-md-6 nasil-calisir-imgs">
                                <img src="@/assets/images/phone.png" alt="phone_png" class="main">
                                <ul class="app-links">
                                    <li>
                                        <router-link to="#">
                                            <img src="@/assets/images/frame2.png" alt="Google_Play">
                                        </router-link>
                                    </li>
                                    <li>
                                        <router-link to="#">
                                            <img src="@/assets/images/frame1.png" alt="Google_Play">
                                        </router-link>
                                    </li>
                                    <li>
                                        <router-link to="#">
                                            <img src="@/assets/images/frame3.png" alt="Google_Play">
                                        </router-link>
                                    </li>

                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>


        <div class="colors-3">
            <div class="blur-1-3 blur"></div>
            <div class="blur-2-3 blur"></div>
            <div class="blur-3-3 blur"></div>
        </div>

        <div>
            <AllTeachers />
        </div>
        <div class="colors-6">
            <div class="blur-2-6 blur"></div>
            <div class="blur-1-6 blur"></div>
        </div>
        <div>
            <NewTeachers />
        </div>
        <div>
            <Upcoming />
        </div>
        <div>
            <BigSlider />
        </div>

        <div class="small-cards" style="margin-top: 45px">
            <div class="container small-cards-container">
                <div class="small-card small-card-1">
                    <p>999'dan daha fazla içerik</p>
                </div>
                <div class="small-card small-card-2">
                    <p>Workshoplar</p>
                </div>
                <div class="small-card small-card-3">
                    <p>Canlı dersler</p>
                </div>
            </div>
        </div>
        <div class="colors-4">
            <div class="blur-2-4 blur"></div>
            <div class="blur-1-4 blur"></div>
        </div>
        <div class="colors-5">
            <div class="blur-2-5 blur"></div>
            <div class="blur-1-5 blur"></div>
        </div>
        <div>
            <Library />
        </div>
        
        <div class="container mt-5">
            <div class="row">
                <div class="col-md-4 p-4">
                    <h3 class="text-white">Lorem Ipsum Dolor.</h3>
                    <p class="text-white">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit!</p>
                    <div class="mt-5">
                        <div class="row">
                            <div class="col-md-6">
                                <button class="faces-kesfet-btn">Keşfet</button>
                            </div>
                            <div class="col-md-6">
                                <router-link to="#" style="text-decoration: none; color: white;">Daha fazla Ogren
                                </router-link>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-md-2"></div>
                <div class="col-md-6">
                    <img src="@/assets/images/faces.png" alt="faces_png" style="width:95%">
                </div>
            </div>
        </div>

        <div>
            <Footer />
        </div>
    </div>
</template>

<script>
import AllTeachers from './AllTeachers.vue';
import PopularEgitmler from './PopularEgitmler.vue';
import TopTen from './TopTen.vue';
import NewTeachers from './NewTeachers.vue';
import Upcoming from './Upcoming.vue';
import BigSlider from './BigSlider.vue';
import Library from './Library.vue';
import Footer from './Footer.vue';
import SmallNav from './SmallNav.vue';
export default {
    name: "HomePage",
    components: { PopularEgitmler, TopTen, AllTeachers, NewTeachers, Upcoming, BigSlider, Library, Footer, SmallNav }
}
</script>

<style>
</style>