<script >

export default {
    name: 'Jumbotron',
};
</script>

<template>
    <section>
        <img src="/jumbotron.jpg" alt="Jumbo">
        <div class="container">
            <h3>Current Series</h3>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as *;

section {
    height: 400px;

    h3 {
        display: inline-block;
        background-color: $blue-dc;
        padding: 0 20px;
        height: 60px;
        line-height: 60px;
        text-transform: uppercase;
        color: white;
        position: relative;
        bottom: 30px;
        left: 0;
    }

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
    }
}
</style>
