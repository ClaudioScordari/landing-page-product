<script>
export default {
    data() {
        return {
            faqs: [
                {
                    textButton: 'Come posso utilizzare la paperella di gomma per il debugging?',
                    answer: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis beatae ea ratione fuga nobis deserunt optio id magnam, magni ad cupiditate labore tenetur perspiciatis commodi atque aut quae ut asperiores velit consequuntur laudantium soluta explicabo voluptates. Architecto dolorum eos voluptatibus alias iste.',
                    idAccordion: 'collapseOne',
                },
                {
                    textButton: 'Quali sono i vantaggi di usare una paperella di gomma per i programmatori?',
                    answer: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis beatae ea ratione fuga nobis deserunt optio id magnam, magni ad cupiditate labore tenetur perspiciatis commodi atque aut quae ut asperiores velit consequuntur laudantium soluta explicabo voluptates. Architecto dolorum eos voluptatibus alias iste.',
                    idAccordion: 'collapseTwo',
                },
                {
                    textButton: 'Posso usare la paperella di gomma indipendentemente dal linguaggio di programmazione che utlizzo?',
                    answer: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis beatae ea ratione fuga nobis deserunt optio id magnam, magni ad cupiditate labore tenetur perspiciatis commodi atque aut quae ut asperiores velit consequuntur laudantium soluta explicabo voluptates. Architecto dolorum eos voluptatibus alias iste.',
                    idAccordion: 'collapseThree',
                },
                {
                    textButton: 'Quanto dettagliatamente devo spiegare il mio codice alla paperella di gomma?',
                    answer: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis beatae ea ratione fuga nobis deserunt optio id magnam, magni ad cupiditate labore tenetur perspiciatis commodi atque aut quae ut asperiores velit consequuntur laudantium soluta explicabo voluptates. Architecto dolorum eos voluptatibus alias iste.',
                    idAccordion: 'collapseFour',
                },
            ]
        };
    },
}
</script>

<template>
    <section id="faqs" class="container">
        <h2 class="fs-1 fw-bold text-center my-4">FAQs</h2>

        <div class="row">
            <div class="col-lg-6 col-sm-12">
                <img class="img-fluid" src="../assets/imgs/single-image2.png" alt="broken">
            </div>

            <div class="col-lg-6 col-sm-12 pt-3">
                <div class="accordion" id="accordionExample">
                    <div class="accordion-item" v-for="faq in faqs">
                        <h2 class="accordion-header">
                            <button class="accordion-button fw-bold fs-4" type="button" data-bs-toggle="collapse" :data-bs-target="'#' + faq.idAccordion" aria-expanded="true" :aria-controls="faq.idAccordion">
                                {{ faq.textButton }}
                            </button>
                        </h2>

                        <div :id="faq.idAccordion" class="accordion-collapse collapse show" data-bs-parent="#accordionExample">
                            <div class="accordion-body lh-base">
                                {{ faq.answer }}
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    // Importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;
</style>
