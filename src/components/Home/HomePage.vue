<template>
    <div class=" position-relative p-0">
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

        <PopularEgitmler/>

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

        <TopTen/>
    </div>
</template>

<script>
import PopularEgitmler from './PopularEgitmler.vue';
import TopTen from './TopTen.vue';
export default {
    name: "HomePage",
    components: { PopularEgitmler, TopTen }
}
</script>

<style>
</style>