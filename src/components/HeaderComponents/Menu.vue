<script >
export default {
    name: 'Menu',
    data() {
        return {
            links: [
                {
                    name: 'Characters',
                    target: 'blank',
                    href: '#',
                },
                {
                    name: 'Comics',
                    target: 'blank',
                    href: '#',
                },
                {
                    name: 'Movies',
                    target: 'blank',
                    href: '#',
                },
                {
                    name: 'Tv',
                    target: 'blank',
                    href: '#',
                },
                {
                    name: 'Games',
                    target: 'blank',
                    href: '#',
                },
                {
                    name: 'Collectibles',
                    target: 'blank',
                    href: '#',
                },
                {
                    name: 'Videos',
                    target: 'blank',
                    href: '#',
                },
                {
                    name: 'Fans',
                    target: 'blank',
                    href: '#',
                },
                {
                    name: 'News',
                    target: 'blank',
                    href: '#',
                },
                {
                    name: 'Shop',
                    target: 'blank',
                    href: '#',
                },
            ]
        }
    },
};
</script>

<template>
    <ul>
        <li v-for="link in links"><a :href="link.href" :target="link.target">{{ link.name }}</a></li>
    </ul>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables' as *;

ul {
    display: flex;
    gap: 35px;
    height: 100%;

    li {
        height: 100%;
    }

    a {
        color: #464646;
        display: inline-block;
        height: 100%;
        line-height: 120px;
        border-top: 5px solid transparent;
        border-bottom: 5px solid transparent;
        text-transform: uppercase;

        &:hover {
            border-bottom: 5px solid $blue-dc;
            color: $blue-dc;
        }
    }
}
</style>
