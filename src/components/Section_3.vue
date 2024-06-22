<script>
export default {
    data() {
        return {
            ducks: [
                {
                    src: 'product-item1.png',
                    name: 'Cool-Duck',
                    price: '$15',
                },
                {
                    src: 'product-item2.png',
                    name: 'Classic-Duck',
                    price: '$29',
                },
                {
                    src: 'product-item3.png',
                    name: 'Bat-Duck',
                    price: '$69',
                },
            ]
        };
    },
    methods:{
        getImagePath: function(imgPath){
            return new URL(imgPath, import.meta.url).href;
        },
    }
}
</script>

<template>
    <section id="section-3">
        <div class="my-container pt-3">
            <h2 class="fs-1 fw-bold">La collezione di paperelle</h2>
    
            <p class="my-5">Una paperella per ogni stile di programmazione</p>

            <div class="row">
                <div class="col-lg-4 col-sm-12" v-for="elem in ducks">
                    <div class="my-card mb-3">
                        <img class="img-fluid" :src="getImagePath('../assets/imgs/'+ elem.src)" alt="rotta">
                    </div>

                    <div class="text-start">
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                        <i class="fa-solid fa-star"></i>
                    </div>

                    <p class="mt-2 fs-3 text-start">
                        {{ elem.name }}
                    </p>

                    <p class="price mt-2 fs-3 text-start fw-bold">
                        {{ elem.price }}
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    // Importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    // GENERAL
    #section-3 {
        background-color: lightgrey;
        text-align: center;
        margin-top: 30px;
    }

    .my-container {
        width: 80%;
        margin: 0 auto;
    }

    .fa-star {
        color: orange;
    }

    .price {
        color: $green-color;
    }
</style>
