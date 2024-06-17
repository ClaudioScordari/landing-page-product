<script>
export default {
    data() {
        return {
            header_links: [
                'Home',
                'I punti di forza',
                'Recensioni',
                'Paperelle',
                'FAQs',
                'Newsletter',
            ]
        };
    },
    methods: {
        // funzione che ritorna il percorso delle img
        getImagePath: function(imgPath){
            return new URL(imgPath, import.meta.url).href;
        },
    }
}
</script>

<template>
    <header class="poppins-regular p-2 pb-4" style="border: 2px solid black;">
        <div class="row align-items-center">
            <!-- logo-duck -->
            <div class="col-lg-5 col-md-6 col-sm" id="duck-logo-col">
                <a href="#nogo" class="d-inline-block img-duck-box">
                    <img :src="getImagePath('../assets/imgs/logo.png')" alt="">
                </a>
            </div>

            <!-- header-links -->
            <div class="col-lg-7 col-md-6 d-none d-lg-block">
                <div class="row">
                    <div class="col" v-for="link in header_links">
                        <a href="#nogo">
                            {{ link }}
                        </a>
                    </div>
                </div>
            </div>

            <!-- hamburger-menu -->
            <div class="col-md-6 col-sm col-md-block d-lg-none" id="hamburger-menu">
                <div class="row justify-content-end pe-4">
                    <button type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasExample" aria-controls="offcanvasExample">
                        <i class="fa-solid fa-bars fa-2xl" style="color: #c3c6d1;"></i>
                    </button>
                </div>

                <!-- off canvas hamburger-menu -->
                <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasExample" aria-labelledby="offcanvasExampleLabel">
                    <div class="offcanvas-header">
                        <a href="#nogo" class="d-inline-block img-duck-box">
                            <img :src="getImagePath('../assets/imgs/logo.png')" alt="">
                        </a>

                        <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close">
                            <i class="fa-solid fa-xmark fa-2xl" style="color: #c3c6d1;"></i>
                        </button>
                    </div>

                    <div class="offcanvas-body">
                        <div class="d-flex flex-column">
                            <a class="d-inline-block py-4" href="#nogo" v-for="link in header_links">
                                {{ link }}
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
    // importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    // GENERAL
    button {
        // tolgo tutto lo stile al bottone
        all: unset;
    }

    // HEADER
    header {
        font-size: 16px;
        font-weight: 400;
        line-height: 1.5;

        a {
            text-decoration: none;
            color: grey;

            &:hover {
                color: $blue-color;
            }
        }
    }

    // font-family
    .poppins-regular {
        font-family: "Poppins", sans-serif;
        font-weight: 400;
        font-style: normal;
    }

    // mediaquery per controllare dispositivi sotto i 576px
    @media (max-width: 575px) {
        #duck-logo-col {
            width: 50%;
        }

        #hamburger-menu {
            width: 50%;
        }
    }
</style>
