<script >
export default {
    name: 'Lists',
    data() {
        return {
            lists: [
                {
                    title: 'Dc comics',
                    links: [
                        {
                            text: 'Characters',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Comics',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Movies',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'TV',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Games',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Videos',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'News',
                            target: 'blank',
                            href: '#',
                        },
                    ]
                },
                {
                    title: 'Shop',
                    links: [
                        {
                            text: 'Shop DC',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Shop DC Collectibles',
                            target: 'blank',
                            href: '#',
                        },
                    ]
                },
                {
                    title: 'Dc',
                    links: [
                        {
                            text: 'Therm of use',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Privacy policy (New)',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Ad Choices',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Advertising',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Jobs',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Subscriptions',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Talent Workshops',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'CPSC Certificates',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Ratings',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Shop Help',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'Contact us',
                            target: 'blank',
                            href: '#',
                        },
                    ]
                },
                {
                    title: 'Sites',
                    links: [
                        {
                            text: 'DC',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'MAD Magazine',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'DC Kids',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'DC Universe',
                            target: 'blank',
                            href: '#',
                        },
                        {
                            text: 'DC Power Visa',
                            target: 'blank',
                            href: '#',
                        },
                    ]
                },
            ]
        }
    },
};
</script>

<template>
    <section>
        <div class="container">
            <nav id="col-left">
                <div class="element" v-for="element in lists">
                    <h5>{{ element.title }}</h5>
                    <ul>
                        <li v-for="link in element.links">
                            <a :href="link.href" :target="link.target">{{ link.text }}</a>
                        </li>
                    </ul>
                </div>
            </nav>
            <img src="../../assets/img/dc-logo-bg.png" alt="Logo Big">
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-image: url('../../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;

    .container {
        height: 370px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        overflow: hidden;

        #col-left {
            height: 100%;
            padding: 40px 0;
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            justify-content: flex-start;

            .element {
                color: white;
                margin-right: 30px;

                h5 {
                    text-transform: uppercase;
                }

                ul {
                    margin: 15px 0 25px 0;

                    a {
                        color: inherit;
                        opacity: .5;


                        &:hover {
                            opacity: 1;
                        }
                    }
                }
            }
        }

        img {
            height: 150%;
        }
    }
}
</style>