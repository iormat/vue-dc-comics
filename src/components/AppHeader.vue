<template>
    <header>
        <div class="top-bar">
            <div class="container-center">
                <img src="../assets/img/dc-logo.png" alt="">
                <section class="header-nav">
                    <nav>
                        <ul>
                            <li v-for="(link, i) in links" :key="i"> 
                                <a :class="link.selected ? 'active' : '' " href="link.url">{{ link.text }}</a> 
                            </li>
                        </ul>
                    </nav>
                </section>
            </div>
        </div>
        <section id="jumbo"></section>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',
    data(){
        return {
            links : [
                {
                    url : "#",
                    text : "characters",
                    selected : false,
                },
                {
                    url : "#",
                    text : "comics",
                    selected : true,
                },
                {
                    url : "#",
                    text : "movies",
                    selected : false,
                },
                {
                    url : "#",
                    text : "tv",
                    selected : false,
                },
                {
                    url : "#",
                    text : "games",
                    selected : false,
                },
                {
                    url : "#",
                    text : "collectibles",
                    selected : false,
                },
                {
                    url : "#",
                    text : "videos",
                    selected : false,
                },
                {
                    url : "#",
                    text : "fans",
                    selected : false,
                },
                {
                    url : "#",
                    text : "news",
                    selected : false,
                },
                {
                    url : "#",
                    text : "shop",
                    selected : false,
                }
            ]
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .top-bar {
        background-color: #fff;
        padding: 20px 0;
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        z-index: 2;

    }
    .container-center {
        display: flex;
        justify-content: space-between;
        align-items: center;
        & img {
            width: 70px;
            display: block;
        }
    }
    li {
        display: inline-block;
        margin: 0 15px;
        & a {
            padding: 40px 0;
            color: #000;
            text-decoration: none;
            font-size: .8rem;
            font-weight: bold;
        }
        & a.active, a:hover {
            color: #377AE4;
            border-bottom: 3px solid #377AE4;
        }
    }

    #jumbo {
        background-image: url('../assets/img/jumbotron.jpg');
        background-position: top;
        background-size: cover;
        height: 500px;
        position: relative;
        top: 100px;
    }
</style>
