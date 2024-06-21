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
    <section id="section-2">
        <h2 class="fs-1 fw-bold text-center">Cosa ne pensano i nostri sviluppatori</h2>

        <!-- swiper-lg -->
        <swiper id="swiper-lg" :slidesPerView="1" :spaceBetween="30" :keyboard="{ enabled: true,}" :pagination="{ clickable: true}" :navigation="true" :modules="modules">
            <swiper-slide>
                <div class="row">
                    <div class="col">
                        <div class="my-card">
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt laborum autem quod explicabo nulla tenetur fuga alias quisquam pariatur temporibus, assumenda necessitatibus aliquid corrupti architecto sint velit illo et amet fugit inventore beatae neque dolorum, numquam sequi. Aliquid, vitae asperiores.</p>

                            <div>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                            </div>

                            <h5 class="fw-bold mt-4">David Wiliam - Feb 22, 2023</h5>
                        </div>
                    </div>
                    <div class="col">
                        <div class="my-card">
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt laborum autem quod explicabo nulla tenetur fuga alias quisquam pariatur temporibus, assumenda necessitatibus aliquid corrupti architecto sint velit illo et amet fugit inventore beatae neque dolorum, numquam sequi. Aliquid, vitae asperiores.</p>

                            <div>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                            </div>

                            <h5 class="fw-bold mt-4">Emma Turner - April 5, 2023</h5>
                        </div>
                    </div>
                    <div class="col">
                        <div class="my-card">
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt laborum autem quod explicabo nulla tenetur fuga alias quisquam pariatur temporibus, assumenda necessitatibus aliquid corrupti architecto sint velit illo et amet fugit inventore beatae neque dolorum, numquam sequi. Aliquid, vitae asperiores.</p>

                            <div>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                            </div>

                            <h5 class="fw-bold mt-4">Rachel Bryan - April 18, 2023</h5>
                        </div>
                    </div>
                </div>
            </swiper-slide>

            <swiper-slide>
                <div class="row">
                    <div class="col">
                        <div class="my-card">
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt laborum autem quod explicabo nulla tenetur fuga alias quisquam pariatur temporibus, assumenda necessitatibus aliquid corrupti architecto sint velit illo et amet fugit inventore beatae neque dolorum, numquam sequi. Aliquid, vitae asperiores.</p>

                            <div>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                            </div>

                            <h5 class="fw-bold mt-4">David Wiliam - Feb 22, 2023</h5>
                        </div>
                    </div>
                    <div class="col">
                        <div class="my-card">
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt laborum autem quod explicabo nulla tenetur fuga alias quisquam pariatur temporibus, assumenda necessitatibus aliquid corrupti architecto sint velit illo et amet fugit inventore beatae neque dolorum, numquam sequi. Aliquid, vitae asperiores.</p>

                            <div>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                            </div>

                            <h5 class="fw-bold mt-4">Emma Turner - April 5, 2023</h5>
                        </div>
                    </div>
                    <div class="col">
                        <div class="my-card">
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt laborum autem quod explicabo nulla tenetur fuga alias quisquam pariatur temporibus, assumenda necessitatibus aliquid corrupti architecto sint velit illo et amet fugit inventore beatae neque dolorum, numquam sequi. Aliquid, vitae asperiores.</p>

                            <div>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                            </div>

                            <h5 class="fw-bold mt-4">Rachel Bryan - April 18, 2023</h5>
                        </div>
                    </div>
                </div>
            </swiper-slide>
        </swiper>

        <!-- swiper-sm -->
        <swiper id="swiper-sm" :slidesPerView="1" :spaceBetween="0" :keyboard="{ enabled: true,}" :pagination="{ clickable: true}" :navigation="true" :modules="modules">
            <swiper-slide>
                <div class="my-card">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt laborum autem quod explicabo nulla tenetur fuga alias quisquam pariatur temporibus, assumenda necessitatibus aliquid corrupti architecto sint velit illo et amet fugit inventore beatae neque dolorum, numquam sequi. Aliquid, vitae asperiores.</p>

                    <div>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                    </div>

                    <h5 class="fw-bold mt-4">David Wiliam - Feb 22, 2023</h5>
                </div>
            </swiper-slide>

            <swiper-slide>
                <div class="my-card">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt laborum autem quod explicabo nulla tenetur fuga alias quisquam pariatur temporibus, assumenda necessitatibus aliquid corrupti architecto sint velit illo et amet fugit inventore beatae neque dolorum, numquam sequi. Aliquid, vitae asperiores.</p>

                    <div>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                    </div>

                    <h5 class="fw-bold mt-4">David Wiliam - Feb 22, 2023</h5>
                </div>
            </swiper-slide>

            <swiper-slide>
                <div class="my-card">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt laborum autem quod explicabo nulla tenetur fuga alias quisquam pariatur temporibus, assumenda necessitatibus aliquid corrupti architecto sint velit illo et amet fugit inventore beatae neque dolorum, numquam sequi. Aliquid, vitae asperiores.</p>

                    <div>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                    </div>

                    <h5 class="fw-bold mt-4">David Wiliam - Feb 22, 2023</h5>
                </div>
            </swiper-slide>

            <swiper-slide>
                <div class="my-card">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt laborum autem quod explicabo nulla tenetur fuga alias quisquam pariatur temporibus, assumenda necessitatibus aliquid corrupti architecto sint velit illo et amet fugit inventore beatae neque dolorum, numquam sequi. Aliquid, vitae asperiores.</p>

                    <div>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                    </div>

                    <h5 class="fw-bold mt-4">David Wiliam - Feb 22, 2023</h5>
                </div>
            </swiper-slide>
        </swiper>
    </section>
</template>

<style lang="scss" scoped>
    // Importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    // GENERAL
    #swiper-lg { // di default
        display: block;
    }

    #swiper-sm { // di default
        display: none;
    }

    #section-2 {
        width: 80%;
        margin: 0 auto;
    }

    #section-2 h2 {
        margin: 70px 0;
    }

    h2 {
        color: $black-color;
    }

    .my-card {
        text-align: center;
        padding: 30px;
    }

    .fa-star {
        color: orange;
    }

    // mediaquery 
    @media (max-width: 767px) {
        #swiper-lg {
            display: none;
        }

        #swiper-sm {
            display: block;
        }
    }

</style>
