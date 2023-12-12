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
        <img :src="image" :alt="title">
        <h4>{{ title }}</h4>
    </li>
</template>
<style lang="scss" scoped></style>