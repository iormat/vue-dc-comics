<template>
    <div class="card">
        <div class="img-window">
            <img :src="cardDetails.thumb" :alt="cardDetails.series">
        </div>
        <h3>{{cardDetails.series}}</h3>
        <p>{{cardDetails.price}}</p>
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
        padding: 10px;
        .img-window {
            height: 200px;
            overflow: hidden;

            img{
                width: 100%;
            }
        }
        h3 {
            font-size: 1.1rem;
        }
        p {
            font-size: .8rem;
        }
    }

</style>