<template>
    <div class="container">
        <div class="card"
        v-for ="( cardItem , index ) in CardsList"
        :key="`cards-${index}`">
        <div class="cover">
            <img :src="cardItem.thumb" :alt="cardItem.series">
        </div>
        <h3>{{cardItem.series}}</h3>
        </div>
        
    </div>

</template>

<script>
export default {
name:'CardComponent',
props:{
    CardsList:Array
}
}
</script>

<style lang="scss" scoped>
.container{
        display: flex;
        flex-wrap: wrap;
        padding-top: 30px;
        .card{
            width: calc(100% / 6);
            padding: 10px;
            .cover{
                width: 150px;
                height: 150px;
                overflow: hidden;
            }
            h3{
                color: white;
            }
        }
}

</style>