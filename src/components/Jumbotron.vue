<script>
export default {
    data() {
        return {

        };
    },
    methods: {
        // ...
    }
}
</script>

<template>
    <!-- Jumbotron -->
    <div id="jumbotron" class="montserrat">
        <div class="jumbo-left">
            <!-- img-duck -->
        </div>

        <div class="jumbo-right text-center d-flex flex-column justify-content-center aling-items-center p-5">
            <h1 class="fw-bold pb-4">
                Rubber Duck Debuggins
            </h1>

            <p class="fs-4">
                Spiegare il codice ad una paperella di gomma aiuta i programmatori a chiarire il penisero e individuare errori nascosti.
            </p>

            <div class="pt-4">
                <a href="#nogo" class="text-decoration-none border border-1 border-dark px-4 py-3 fs-3">
                    ACQUISTALA SUBITO! 
                </a>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    // importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    #jumbotron {
        height: 600px;
        display: flex;
    }

    .jumbo-left,
    .jumbo-right {
        width: 50%;
        height: 100%;
    }

    .jumbo-left {
        background-image: url('../assets/imgs/banner-image.png');
        background-position: center;
        background-size: cover;

    }

    .jumbo-right {
        background-image: url('../assets/imgs/banner-bg.png');
        background-position: center;
        background-size: cover;

        h1 {
            color: $black-color;
            font-size: 60px;
        }

        div > a {
            color: $black-color;

            &:hover {
                background-color: black;
                color: white;
            }
        }
    }

    // mediaquery 
    @media (max-width: 991px) {
        .jumbo-left,
        .jumbo-right {
            width: 100%;
            height: 100%;
        }

        #jumbotron {
            height: 600px;
            display: block;
        }
    }
</style>
