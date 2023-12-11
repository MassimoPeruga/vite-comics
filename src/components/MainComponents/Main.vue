<script >
import Content from './Content.vue';
import LinkIcons from './LinkIcons.vue';
import Jumbotron from './Jumbotron.vue';
export default {
    name: 'Main',
    components: {
        Content,
        LinkIcons,
        Jumbotron,
    },
};
</script>

<template>
    <main>
        <Jumbotron />
        <Content />
        <LinkIcons />
    </main>
</template>

<style lang="scss"></style>
