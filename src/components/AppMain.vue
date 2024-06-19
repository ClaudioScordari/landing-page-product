<script>
import Jumbotron from './Jumbotron.vue';

export default {
    data() {
        return {

        };
    },
    methods: {
        
    },
    components: {
        Jumbotron
    }
}
</script>

<template>
    <main class="montserrat">
        <Jumbotron />
    </main>
</template>

<style lang="scss" scoped>
    // importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    // ...

</style>
