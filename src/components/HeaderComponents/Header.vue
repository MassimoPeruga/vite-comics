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
    <div class="container">
        <header>
            <Logo />
            <Menu />
        </header>
    </div>
</template>

<style lang="scss">
header {
    height: 120px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
</style>
