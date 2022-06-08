<template>
    <div>
        <div class="container-jumbotron footer-container">
            <div class="footer-light"></div>
            <div class="container">
                <ul class="footer-ul footer-1">
                    <li class="logo">
                            <img src="@/assets/images/logo.png" alt="logo">
                            <span class="yasam-text">yaşam</span> <span class="atolye-text-one">atölyesi</span>
                    </li>
                    <li>
                        <router-link to="#">+1 800 854-80</router-link>
                    </li>
                    <li class="social-icons">
                        <ul>
                            <li class="social-icons-one">
                               <i class="fa-brands fa-facebook-square"></i>
                            </li>
                            <li>
                              <i class="fa-brands fa-instagram-square"></i>
                            </li>
                            <li>
                              <i class="fa-brands fa-github-square"></i>
                            </li>
                            <li>
                              <i class="fa-brands fa-linkedin"></i>
                            </li>
                            <li>
                              <i class="fa-solid fa-paper-plane"></i>
                            </li>
                        </ul>
                    </li>
                    <li>
                        <button class="bize-ulas-btn">Bize ulaş</button>
                    </li>
                </ul>
                <ul class="footer-ul footer-2">
                    <li>
                        Keşfet
                    </li>
                    <li>
                        <router-link to="#">Eğitimler</router-link>
                    </li>
                    <li>
                        <router-link to="#">Eğitmenlerimiz</router-link>
                    </li>
                    <li>
                        <router-link to="#">
                            Planlar
                        </router-link>

                    </li>
                    <li>
                        <router-link to="#">
                            <span class="atolye-text">Atölye</span> +
                        </router-link>
                    </li>
                </ul>
                <ul class="footer-ul footer-2">
                    <li>
                        Hakkımıza
                    </li>
                    <li>
                        <router-link to="#">
                            Yaşam atölyesi nedir?
                        </router-link>
                    </li>
                    <li>
                        <router-link to="#">
                            Kullancı sözleşmesi
                        </router-link>
                    </li>
                    <li>
                        <router-link to="#">
                            Gizililik politikası
                        </router-link>
                    </li>
                    <li>
                        <router-link to="#">
                            Mesafeli Satiş Sözleşme
                        </router-link>
                    </li>

                </ul>
                <ul class="footer-ul footer-4">
                    <li>
                        Destek
                    </li>
                    <li>
                        <router-link to="#">
                            Sıkça Sorun Sorular
                        </router-link>
                    </li>
                    <li>
                        <router-link to="#">
                            Bize Ulaş
                        </router-link>
                    </li>

                </ul>
                <ul class="footer-ul footer-5">
                    <li>
                        Iletişim
                    </li>
                    <li>
                        <router-link to="#">
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus, odit!
                        </router-link>
                    </li>
                    <li>
                        <router-link to="#">
                            +1 800 854-2665
                        </router-link>
                    </li>

                </ul>
            </div>
        </div>
        <div class="right-reserved">
            <div class="container">
                <span class="text-white year-span">&#xa9; {{ new Date().getFullYear() }} All Rights Reserved</span>
                <span class="text-white to-top float-end" @click="scrollTop"><i class="fa-solid fa-angle-up"></i></span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Footer',
    methods: {
        scrollTop() {
            document.body.scrollTop = 0;
            document.documentElement.scrollTop = 0;
        }
    },
}
</script>

<style>
</style>