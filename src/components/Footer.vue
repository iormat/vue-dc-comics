<template>
    <footer>
        <!-- footer up -->
        <section class="foot_up">
            <div class="footup-left">
                <section class="footer-nav">
                    <nav>
                        <h3>DC COMICS</h3>
                    </nav>
                </section>
            </div>
            <div class="footup-right">
                <img src="../assets/img/dc-logo-bg.png" alt="logo dc">
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
    name : "Footer",
    data() {
        return {
            links : [
                {
                    title : "dc comics",
                    url : "#",
                    text : "characters",
                },
                {
                    title : "dc comics",
                    url : "#",
                    text : "comics",
                },
                {
                    title : "dc comics",
                    url : "#",
                    text : "movies",
                },
                {
                    title : "dc comics",
                    url : "#",
                    text : "tv",
                },
                {
                    title : "dc comics",
                    url : "#",
                    text : "games",
                },
                {
                    title : "dc comics",
                    url : "#",
                    text : "videos",
                },
                {
                    title : "dc comics",
                    url : "#",
                    text : "news",
                },
                {
                    title : "shop",
                    url : "#",
                    text : "shop dc",
                },
                {
                    title : "shop",
                    url : "#",
                    text : "shop dc collectibles",
                },

            ]
        }
    }
}
</script>

<style scoped lang="scss">
    footer {
        margin-top: 330px;
        background-image: url('../assets/img/footer-bg.jpg');
        background-size: cover;
        color: #fff;
        & .footup-left {
            width: 50%;
        }
    }
    .foot_up {
        display: flex;
    }

    .foot_down {
        padding: 20px 0;
        background-color: #303030;

        & .container-center {
            display: flex;
            justify-content: space-between;
            flex-flow: row nowrap;
            align-items: center;

            & button a {
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
                & img {
                    margin: 10px;
                }
            }
        }
    }
</style>
