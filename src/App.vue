<script >
import Header from './components/HeaderComponents/Header.vue';
import Footer from './components/FooterComponents/Footer.vue';
export default {
    name: 'App',
    components: {
        Header,
        Footer,
    }
};
</script>

<template>
    <Header />
    <Footer />
</template>

<style lang="scss">
@use './scss/style.scss' as *;
@use './scss/_partials/variables.scss' as *;
</style>
