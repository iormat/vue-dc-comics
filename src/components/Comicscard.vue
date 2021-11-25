<template>
    <div class="card">
        <a href="#">
            <div class="img-window">
                <img :src="cardDetails.thumb" :alt="cardDetails.series">
            </div>
            <h3>{{cardDetails.series}}</h3>
            <p>{{cardDetails.price}}</p>
        </a>
    </div>
</template>


<script>
export default {
    name : 'Comicscard',
    props : {
        cardDetails : Object, 
    }
}
</script>

<style scoped lang="scss">
    .card {
        width: calc(100% / 6);
        min-width: 170px;
        padding: 10px;
        a {
            color: #fff;
            text-decoration: none;
            & .img-window  {
                height: 200px;
                overflow: hidden;
                img { 
                    width: 100%;
                    &:hover {
                        transform: scale(1.2);
                        opacity: .5;
                        transition: linear .2s;
                    }
                }
            }
            & h3 {
                font-size: 1rem;
            }
            & p {
                font-size: .8rem;
                line-break: auto;
            }
        }
    }
</style>