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
        <div class="row h-100">
            <div class="col-md-6 col-sm-12 p-0 h-100">
                <div class="h-100 jumbo-left">

                </div>
            </div>

            <div class="col-md-6 col-sm-12 p-0 h-100">
                <div class="jumbo-right h-100 p-5 text-center">
                    <h1>
                        Rubber Duck Debuggings
                    </h1>

                    <p class="my-5 fs-3">
                        Spiegare il codice ad una paperella di gomma aiuta i programmatori a chiarire il pensiero e a individuare errori nascosti.
                    </p>

                    <div>
                        <a class="text-decoration-none border border-1 border-dark px-4 py-3 fs-3" href="#nogo">
                            ACQUISTA SUBITO
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    // importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    // GENERAL
    #jumbotron {
        // altezza fissa del jumbotron
        height: 688px;
    }

    .jumbo-right {
        background-image: url('../assets/imgs/banner-bg.png');
        background-position:center;
        background-size: cover;

        h1 {
            color: $black-color;
            font-size: 80px;
        }

        div > a {
            color: $black-color;

            &:hover {
                background-color: black;
                color: white;
            }
        }
    }

    .jumbo-left {
        background-image: url('../assets/imgs/banner-image.png');
        background-position:center;
        background-size: cover;
    }

</style>
