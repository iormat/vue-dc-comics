<template>
    <main>
        <section id="comics"></section>
        <!-- section cards -->
        <section id="cards">
            <ul class="container-center">
                <li v-for="card, i in cards" :key="i">
                    <a href="#">
                        <img :src="card.image" :alt="card.title">
                        <p>{{ card.title }}</p>
                    </a>
                </li>
            </ul>
        </section>
    </main>
</template>


<script>
export default {
    name : 'Main',
    data(){
        return{
            cards : [
                {
                    title : 'digital comics',
                    image : "./img/buy-comics-digital-comics.png"
                },
                {
                    title : 'dc merchandise',
                    image : './img/buy-comics-merchandise.png'
                },
                {
                    title : 'subscription',
                    image : './img/buy-comics-subscriptions.png'
                },
                {
                    title : 'comic shop locator',
                    image : './img/buy-comics-shop-locator.png'
                },
                {
                    title : 'dc power visa',
                    image : './img/buy-dc-power-visa.svg'
                },
            ],
        }
    }
}
</script>

<style scoped lang="scss">
#cards {
    margin-top: 200px;
    background-color: #3880F1;
    & ul {
        display: flex;
        justify-content: space-around;
        align-items: center;
        & li {
            list-style: none;
            & a {
                width: 20%;
                display: flex;
                align-items: center;
                color: #fff;
                text-decoration: none;
                padding: 20px 0;
                & img {
                    width: 50px;
                    height: 50px;
                    margin-right: 5px;
                }
                & p {
                    font-size: 1rem;
                    white-space: nowrap;
                }
            }
        }
    }
}
</style>