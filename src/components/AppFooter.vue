<script>
export default {
    data() {
        return {
            icons: [
                'fa-brands fa-facebook-f fa-2xl',
                'fa-brands fa-instagram fa-2xl',
                'fa-brands fa-youtube fa-2xl',
                'fa-brands fa-linkedin fa-2xl',
                'fa-brands fa-twitter fa-2xl',
            ]
        };
    },
}
</script>

<template>
    <footer class="montserrat text-center">
        <section id="footer-top" class="p-4">
            <div class="container">
                <h2>
                    Iscriviti per rimanere aggiornato
                </h2>

                <p class="my-5">
                    Iscriviti alla nostra newsletter per rimanere aggiornato su sconti e novità
                </p>

                <form class="w-50 mx-auto d-flex justify-content-between align-items-center mb-5" action="">
                    <input class="w-100 p-3" type="email" placeholder="Inserisci la tua email qui...">

                    <button class="d-inline-block p-3">
                        <i class="fa-regular fa-paper-plane fa-2xl"></i>
                    </button>
                </form>  

                <div id="icons-box" class="d-inline-block mx-auto mt-2 d-flex justify-content-between align-items-center">
                    <a class="rounded-circle" v-for="icon in icons" href="#nogo" style="width: 60px; height: 60px; line-height: 60px;">
                        <i :class="icon"></i>
                    </a>
                </div>              
            </div>
        </section>

        <section id="footer-bottom" class="p-4 text-center">
            C 2024 BooLanding Product. Designed by Boolean
        </section>
    </footer>
</template>

<style lang="scss" scoped>
    // importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    // GENERAL
    #footer-top {
        background-color: lightgray;
    }

    #icons-box {
        width: 30%;
    }

    h2 {
        font-size: 50px;
        width: 50%;
        margin: 0 auto;
        color: $black-color;
        font-weight: bold;
    } 

    form {
        border-bottom: 1px solid grey;
    }

    input {
        border: none;
        display: inline-block;
        background-color: lightgray;
    }

    a {
        text-decoration: none;
        border: 1px solid grey;
    }

    form button {
        background-color: lightgray;
        border: none;
    }

    form i,
    i {
        color: $green-color;
    }

    // mediaquery
    @media (max-width: 992px) {
        #icons-box {
            width: 60%;
            margin: 0 auto;
        }
    }
</style>
