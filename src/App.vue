<script>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import AppMain from './components/AppMain.vue';

export default {
    data() {
        return {

        };
    },
    methods: {
        // ...
    },
    components: {
        AppHeader,
        AppMain,
        AppFooter,
    }
}
</script>

<template>
    <AppHeader/>

    <AppMain/>

    <AppFooter/>
</template>

<style lang="scss" scoped>
@use 'assets/scss/main.scss' as *;

</style>

