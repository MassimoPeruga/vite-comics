<script >
export default {
    name: 'Logo',
    data() {
        return {
            image: {
                alt: 'Logo',
                url: 'dc-logo.png',
            },
        };
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(imgPath, import.meta.url).href;
        },
    },
};
</script>

<template>
    <img :src="getImagePath(`../../assets/img/${image.url}`)" :alt="image.alt">
</template>

<style lang="scss" scoped>
img {
    display: block;
    height: 80px;
}
</style>
