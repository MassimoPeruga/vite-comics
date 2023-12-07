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
@use '../../scss/_partials/variables.scss' as *;

ul {
    list-style: none;
    display: flex;
    gap: 35px;

    a {
        text-decoration: none;
        color: #464646;
        display: inline-block;
        height: 100%;
        line-height: 120px;
        border-bottom: 5px solid transparent;

        &:hover {
            border-color: $blue-dc;
            color: $blue-dc;
        }
    }
}
</style>
