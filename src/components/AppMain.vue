<script>
import Jumbotron from './Jumbotron.vue';
import Section_1 from './Section_1.vue';


export default {
    data() {
        return {

        };
    },
    methods: {
        
    },
    components: {
        Jumbotron,
        Section_1
    }
}
</script>

<template>
    <main class="montserrat">
        <Jumbotron />

        <Section_1 />
    </main>
</template>

<style lang="scss" scoped>
    // importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    // ...

</style>
