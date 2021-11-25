<template>
    <footer>
        <!-- footer up -->
        <section class="foot_up container-center">
            <!-- left footer top section -->
            <div class="footup-left">
                <section class="footer-nav">
                    <!-- nav dc comics and shop -->
                    <nav>
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="link, i in dcComicsArr" :key="i">
                                <a href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                        <!-- nav shop -->
                        <h3>SHOP</h3>
                        <ul>
                            <li v-for="link, i in shopArr" :key="i">
                                <a href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </nav>
                    <!-- nav dc -->
                    <nav>
                        <h3>DC</h3>
                        <ul>
                            <li v-for="link, i in dcArr" :key="i">
                                <a href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </nav>
                    <!-- nav sites -->
                    <nav>
                        <h3>SITES</h3>
                        <ul>
                            <li v-for="link, i in sitesArr" :key="i">
                                <a href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </nav>
                </section>
            </div>
            <!-- right footer top section -->
            <div class="footup-right">
            </div>
        </section>
        <!-- footer down -->
        <section class="foot_down">
            <div class="container-center">
                <button class="btn footer-btn">
                    <a href="#"> SIGN&minus;IN NOW&excl; </a>
                </button>
                <!-- social footer section -->
                <section class="social">
                    <h3>FOLLOW US</h3>
                    <!-- social links icons -->
                    <a href="#">
                        <img src="../assets/img/footer-facebook.png" alt="facebook logo">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-twitter.png" alt="facebook logo">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-youtube.png" alt="facebook logo">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-pinterest.png" alt="facebook logo">
                    </a>
                    <a href="#">
                        <img src="../assets/img/footer-periscope.png" alt="facebook logo">
                    </a>
                </section>
            </div>
        </section>
    </footer>
</template>

<script>
export default {
    name : "AppFooter",
    data() {
        return {
            dcComicsArr : [
                {
                    url : "#",
                    text : "characters",
                },
                {
                    url : "#",
                    text : "comics",
                },
                {
                    url : "#",
                    text : "movies",
                },
                {
                    url : "#",
                    text : "tv",
                },
                {
                    url : "#",
                    text : "games",
                },
                {
                    url : "#",
                    text : "videos",
                },
                {
                    url : "#",
                    text : "news",
                },
            ],
            shopArr : [
                {
                    url : "#",
                    text : "shop dc",
                },
                {
                    url : "#",
                    text : "shop dc collectibles",
                },
            ],
            dcArr : [
                {
                    url : "#",
                    text : "therms of use",
                },
                {
                    url : "#",
                    text : "Privacy policy (New)",
                },
                {
                    url : "#",
                    text : "Ad Choices",
                },
                {
                    url : "#",
                    text : "Advertising",
                },
                {
                    url : "#",
                    text : "jobs",
                },
                {
                    url : "#",
                    text : "Subscriptions",
                },
                {
                    url : "#",
                    text : "Talent Workshops",
                },
                {
                    url : "#",
                    text : "CPSC Certificates",
                },
                {
                    url : "#",
                    text : "Ratings",
                },
                {
                    url : "#",
                    text : "Shop Help",
                },
                {
                    url : "#",
                    text : "Contact Us",
                },
            ],
            sitesArr : [
                {
                    url : "#",
                    text : "dc",
                },
                {
                    url : "#",
                    text : "MAD Magazine",
                },
                {
                    url : "#",
                    text : "DC kids",
                },
                {
                    url : "#",
                    text : "DC Universe",
                },
                {
                    url : "#",
                    text : "DC Power Visa",
                },
            ]
        }
    },
}
</script>

<style scoped lang="scss">
    footer {
        background-image: url('../assets/img/footer-bg.jpg');
        background-size: cover;
        color: #fff;
    }

    .foot_up {
        display: flex;
        & .footup-left {
            width: 50%;
            padding: 30px 0;
            & .footer-nav {
                display: flex;
                & h3 {
                    margin: 20px 0;
                    font-size: 1.2rem
                }
            }
        }
        & nav {
            margin: 0 30px;
        }
        a {
            text-transform: capitalize;
            text-decoration: none;
            color: #878585;
            font-size:.8rem;
        }
        a:hover {
            text-decoration: underline;
        }


        & nav ul li {
            list-style: none;
        }
    }

    .footup-right {
        background-image: url("../assets/img/dc-logo-bg.png");
        background-size: cover;
        background-position: center;
        width: 50%;
    }

    .foot_down {
        padding: 20px 0;
        background-color: #303030;

        & .container-center {
            display: flex;
            justify-content: space-between;
            flex-flow: row nowrap;
            align-items: center;
            button {
                background-color: transparent;
                &:hover {
                    background-color: hsl(0, 0%, 50%);
                    cursor: pointer;
                }
            }
            & button a {
                padding: 10px 15px;
                color: #fff;
                text-decoration: none;
                font-size: 1.2rem;
                font-weight: bold;
                cursor: pointer;
            }
            & .social {
                color: #3874D9;
                display: flex;
                align-items: center;
                & h3 {
                    margin-right: 10px;
                }
                & a {
                    margin: 10px;
                }
            }
        }
    }
</style>
