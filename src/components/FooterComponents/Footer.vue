<script >
import Lists from './Lists.vue';
import Buttons from './Buttons.vue';
export default {
    name: 'Footer',
    components: {
        Lists,
        Buttons,
    }
};
</script>

<template>
    <footer>
        <Lists />
        <Buttons />
    </footer>
</template>

<style lang="scss">
@use '../../scss/_partials/variables.scss' as *;
</style>