<script >

export default {
    name: 'Jumbotron',
};
</script>

<template>
    <section>
        <img src="/jumbotron.jpg" alt="Jumbo">
    </section>
</template>

<style lang="scss" scoped>
section {
    height: 400px;

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
    }
}
</style>
