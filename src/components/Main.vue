<template>
    <main>
        <section id="comics">
            <h2>current series</h2>
            <section id="comics-cards" class="container-center">
                <Comicscard v-for="comicsCard, j in comicsArr" :key="j"
                    :cardDetails="comicsCard"/>
            </section>
        </section>
        <!-- section cards -->
        <section id="link-cards">
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
import Comicscard from "./Comicscard.vue";

export default {
    name : 'Main',
    components: {
        Comicscard,
    },
    data(){
        return{
            // useful links
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
            // comics cards
            comicsArr: [
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    },
}
</script>

<style scoped lang="scss">
main {
    background-color: #000;
    padding-top: 30px;
}
#comics {
    margin-top: 50px;
    color: #fff;
        h2 {
            background-color: #3880F1;
            margin-left: 10%;
            padding: 5px 20px;
            box-shadow: 5px 0 5px rgba(1, 1, 1, 0.397);
            display: inline;
            position: relative;
            z-index: 1;
        }

    #comics-cards {
        padding: 30px 0;
        display: flex;
        flex-flow: row wrap;
    }
}

#link-cards {
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