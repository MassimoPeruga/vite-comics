<script >
export default {
    name: 'LinkIcons',
    data() {
        return {
            links: [
                {
                    name: 'Digital Comics',
                    target: 'blank',
                    href: '#',
                    icon: {
                        alt: 'Digital Icon',
                        url: 'buy-comics-digital-comics.png',
                    }
                },
                {
                    name: 'Dc Merchandise',
                    target: 'blank',
                    href: '#',
                    icon: {
                        alt: 'Merchandise Icon',
                        url: 'buy-comics-merchandise.png',
                    }
                },
                {
                    name: 'Subscription',
                    target: 'blank',
                    href: '#',
                    icon: {
                        alt: 'Subscription Icon',
                        url: 'buy-comics-subscriptions.png',
                    }
                },
                {
                    name: 'Comic Shop Locator',
                    target: 'blank',
                    href: '#',
                    icon: {
                        alt: 'Shop Locator Icon',
                        url: 'buy-comics-shop-locator.png',
                    }
                },
                {
                    name: 'Dc Power Visa',
                    target: 'blank',
                    href: '#',
                    icon: {
                        alt: 'Powe Visa Icon',
                        url: 'buy-dc-power-visa.svg',
                    }
                },
            ]
        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(imgPath, import.meta.url).href;
        },
    },
};
</script>

<template>
    <section>
        <ul class="container">
            <li v-for="link in links">
                <a :href="link.href">
                    <img :src="getImagePath(`../../assets/img/${link.icon.url}`)" :alt="link.icon.alt"
                        :class="{ visa: link.name === 'Dc Power Visa' }">
                </a>
                <a :href="link.href">{{ link.name }}</a>
            </li>
        </ul>
    </section>
</template>

<style lang="scss" scoped>
@use '../../scss/_partials/variables.scss' as *;

section {
    background-color: $blue-dc;
}

ul {
    display: flex;
    list-style: none;
    height: 155px;
    justify-content: space-between;
    align-items: center;
}

li {
    height: 50%;
    display: flex;
    gap: 16px;
}

img {
    display: block;
    height: 100%;

    &.visa {
        height: calc(100% - 20px);
    }
}

a {
    height: 100%;
    text-decoration: none;
    text-transform: uppercase;
    color: white;
    display: flex;
    align-items: center;
}
</style>
