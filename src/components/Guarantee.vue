<script>
export default {
    data() {
        return {
            datas: [
                {
                    iconClass: 'fa-regular fa-lightbulb fs-1',
                    title: '100% Prodotto di qualità',
                    text: 'Abbiamo possibilità di ritiro direttamente dallo stagno',
                },
                {
                    iconClass: 'fa-solid fa-bag-shopping fs-1',
                    title: 'Spedizione gratuita',
                    text: 'Dal magazzino alla scrivania',
                },
                {
                    iconClass: 'fa-solid fa-bandage fs-1',
                    title: 'Rimborso garantito',
                    text: 'Ti rimborsiamo se la paperella fa quack',
                },
            ]
        };
    },
}
</script>

<template>
    <section id="guarantee" class="container py-5 text-center">
        <div class="row">
            <div class="col-lg-4 col-sm-12" v-for="data in datas">
                <i :class="data.iconClass"></i>
                
                <h2 class="fw-bold fs-4 my-2">{{ data.title }}</h2>

                <p>{{ data.text }}</p>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    // Importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    // GENERAL
    #guarantee {
        margin-bottom: 80px;
    }

    i {
        color: $blue-color;
        display: inline-block;
    }

    .row > .col-lg-4.col-sm-12:nth-of-type(2) {
        border-right: 1px solid lightgrey;
        border-left: 1px solid lightgrey;
    }

    // mediaquery 
    @media (max-width: 992px) {
        .row > .col-lg-4.col-sm-12:nth-of-type(2) {
            border: none;
            margin: 30px 0;
        }
    }
</style>
