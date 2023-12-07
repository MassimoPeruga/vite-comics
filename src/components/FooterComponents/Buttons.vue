<script >
export default {
    name: 'Buttons',
    data() {
        return {
            links: [
                {
                    target: 'blank',
                    href: '#',
                    icon: {
                        alt: 'Facebook Icon',
                        url: 'footer-facebook.png',
                    }
                },
                {
                    target: 'blank',
                    href: '#',
                    icon: {
                        alt: 'Twitter Icon',
                        url: 'footer-twitter.png',
                    }
                },
                {
                    target: 'blank',
                    href: '#',
                    icon: {
                        alt: 'YouTube Icon',
                        url: 'footer-youtube.png',
                    }
                },
                {
                    target: 'blank',
                    href: '#',
                    icon: {
                        alt: 'Pinterest Icon',
                        url: 'footer-pinterest.png',
                    }
                },
                {
                    target: 'blank',
                    href: '#',
                    icon: {
                        alt: 'Periscope Icon',
                        url: 'footer-periscope.png',
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
        <div class="container">
            <button>
                <a href="#">Sign-up now!</a>
            </button>
            <div class="flex">
                <h5>Follow us</h5>
                <ul>
                    <li v-for="link in links">
                        <a :href="link.href" :target="link.target">
                            <img :src="getImagePath(`../../assets/img/${link.icon.url}`)" :alt="link.icon.alt">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../scss/_partials/variables.scss' as *;

section {
    background-color: #303030;
    color: white;
    text-transform: uppercase;

    .container {
        height: 110px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        button {
            all: unset;

            a {
                text-decoration: none;
                color: inherit;
                padding: 15px;
                border: 2px solid $blue-dc;
            }
        }

        .flex {
            display: flex;
            align-items: center;
            gap: 25px;

            h5 {
                color: $blue-dc;
            }

            ul {
                list-style: none;
                display: flex;
                align-items: center;
                gap: 15px;

                img {
                    display: block;
                    width: 35px;
                }
            }
        }
    }
}
</style>
