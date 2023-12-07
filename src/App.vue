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
    <div id="container">
        <Header />
        <Footer />
    </div>
</template>

<style lang="scss">
@use './scss/style.scss' as *;
@use './scss/_partials/variables.scss' as *;

#container {
    width: 70%;
    margin: 0 auto;
}
</style>
