<script >
import Header from './components/HeaderComponents/Header.vue';
import Main from './components/MainComponents/Main.vue';
import Footer from './components/FooterComponents/Footer.vue';
export default {
    name: 'App',
    components: {
        Header,
        Footer,
        Main,
    }
};
</script>

<template>
    <Header />
    <Main />
    <Footer />
</template>