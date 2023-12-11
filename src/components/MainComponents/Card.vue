<script >
export default {
    name: 'Card',
    props: {
        image: String,
        title: String,
    }
};
</script>

<template>
    <li>
        <div class="image-container">
            <img :src="image" :alt="title">
        </div>
        <h4>{{ title }}</h4>
    </li>
</template>
<style lang="scss" scoped></style>