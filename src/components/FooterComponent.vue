<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="flex">
                    <div class="company-contacts">
                        <div class="logo">
                            <a @click.prevent href="#">
                                <span class="nex-wrapper">NEX</span>
                                <span class="gen-wrapper">GEN</span>
                            </a>
                        </div>
                        <p>A Functional HTML Template for Corporate & Business.</p>
                        <ul class="contacts-list">
                            <li>
                                <a @click.prevent href="#">
                                    <span>
                                        <i class="fa-solid fa-phone"></i>
                                    </span>
                                    +1 (305) 1234-5678
                                </a>
                            </li>
                            <li>
                                <a @click.prevent href="#">
                                    <span>
                                        <i class="fa-solid fa-envelope"></i>
                                    </span>
                                    hello@example.com
                                </a>
                            </li>
                            <li>
                                <a @click.prevent href="#">
                                    <span>
                                        <i class="fa-solid fa-location-dot"></i>
                                    </span>
                                    Main Avenue, 987
                                </a>
                            </li>
                        </ul>
                        <a @click.prevent href="#" class="btn transparent white">GET IN TOUCH</a>
                    </div>
                    <div class="footer-top-right flex wrap">
                        <div class="footer-links" v-for="element in footerLinks" :key="element.id">
                            <h3>
                                {{element.title}}
                            </h3>
                            <ul>
                                <li v-for="(element, index) in element.links" :key="index">
                                    <a @click.prevent href="#">
                                        <span class="list-chevron">
                                            <i class="fa-solid fa-chevron-right"></i>
                                        </span>
                                        {{element}}
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <div class="flex justify-between">
                    <p>Enjoy the low price. We are tracking any intention of piracy.</p>
                    <p>
                        <span>&#169;</span>
                        2020 NEXGEN is Proudly Powered by
                        <a @click.prevent href="#">Codings</a>.
                    </p>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
// *IMPORTS

export default {
    name: "FooterComponent",
    components: {

    },
    props: {
        footerLinks: Array,
    },
    data() {
        return {

        }
    },
    methods: {

    },
}
</script>

<style lang="scss" scoped>
// *IMPORTS
@import "../style/variables.scss";

// *STYLING
footer {
    color: $second-color;
}
.footer-top {
    padding-block: $footer-padding;
    background-color: $first-color;

    .container > .flex {
        gap: 2rem;
    }
    .company-contacts {
        width: calc((100% / 4) - 1rem);
    }
    .footer-top-right {
        width: calc(100% - ((100% / 4) - 1rem));
        gap: 1.2rem;
    }
    :is(li) {
        font-size: 0.7rem;
        font-weight: 200;
    }
}
.company-contacts {

    .logo {
        margin-bottom: 1rem;
    }
    p {
        margin-bottom: 1.4rem;;
    }
    .contacts-list {
        margin-bottom: 1.4rem;

        li {
            margin-bottom: 0.7rem;

            &:last-of-type {
                margin-bottom: 0;
            }
            a > span {
                margin-right: 0.4rem;
            }
        }
    }
}
.footer-links {
    padding: 1.9rem;
    width: calc((100% / 3) - 0.8rem);
    border-radius: 0.4rem;
    background-color: #19191f;

    h3 {
        margin-bottom: 0.9rem;
    }
    li {
        margin-bottom: 0.45rem;

        .list-chevron {
            margin-right: 0.3rem;
        }
    }
}
.footer-bottom {
    padding-block: 1.4rem;
    background-color: #0d0d11;

    p {
        margin-bottom: 0;
        font-size: 0.6rem;

        > a {
            color: $third-color;

            &:hover {
                text-decoration: underline;
            }
        }
    }
}
</style>