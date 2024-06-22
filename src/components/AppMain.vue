<script>
import Jumbotron from './Jumbotron.vue';
import Section_1 from './Section_1.vue';
import Section_2 from './Section_2.vue';
import Section_3 from './Section_3.vue';
import FAQs from './FAQs.vue';
import Guarantee from './Guarantee.vue';

export default {
    data() {
        return {

        };
    },
    methods: {
        
    },
    components: {
        Jumbotron,
        Section_1,
        Section_2,
        Section_3,
        FAQs,
        Guarantee
    }
}
</script>

<template>
    <main class="montserrat">
        <Jumbotron />

        <Section_1 />

        <Section_2 />

        <Section_3 />

        <FAQs />

        <Guarantee />
    </main>
</template>

<style lang="scss" scoped>
    // importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    // ...

</style>
