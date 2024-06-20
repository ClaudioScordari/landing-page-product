<script>
  // Import Swiper Vue.js components
  import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
  import 'swiper/css';
  import 'swiper/css/pagination';
  import { Keyboard, Pagination, Navigation } from 'swiper/modules';


  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
        return {
            modules: [Keyboard, Pagination, Navigation],
        };
    },
  };
</script>

<template>
    <section id="section-2" class="border border-1 border-dark">
        <h2 class="fs-1 fw-bold text-center">Cosa ne pensano i nostri sviluppatori</h2>

        <!-- swiper -->
        <swiper id="swiper" :slidesPerView="1" :spaceBetween="30" :keyboard="{ enabled: true,}" :pagination="{ clickable: true}" :navigation="true" :modules="modules">
            <swiper-slide>
                <!-- slide 1 -->
            </swiper-slide>

            <swiper-slide>
                <!-- slide 2 -->
            </swiper-slide>
        </swiper>
    </section>
</template>

<style lang="scss" scoped>
    // Importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    // GENERAL
    h2 {
        color: $black-color;
    }
</style>
