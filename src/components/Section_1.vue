<script>
export default {
    data() {
        return {
            
        };
    },
    methods: {
        
    }
}
</script>

<template>
    <section id="section-1">
        <div class="row">
            <div class="col-md-4 col-sm-12">ciao</div>
            <div class="col-md-4 col-sm-12">ciao</div>
            <div class="col-md-4 col-sm-12">ciao</div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    // importazioni variabili e mixins
    @use '../assets/scss/partials/variables.scss' as *;
    @use '../assets/scss/partials/mixins.scss' as *;

    // mediaquery 
    @media (max-width: 991px) {
        #section-1 {
            padding-top: 600px;
        }
    }
</style>
