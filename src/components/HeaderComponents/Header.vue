<script >
import Logo from './Logo.vue';
import Menu from './Menu.vue';
export default {
    name: 'Header',
    components: {
        Logo,
        Menu,
    },
};
</script>

<template>
    <header>
        <Logo />
        <Menu />
    </header>
</template>

<style lang="scss">
header {
    height: 120px;
    display: flex;
    align-items: center;
    justify-content: space-around;
}
</style>
