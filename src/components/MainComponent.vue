<template>
    <main>
        <div class="title">CURRENT SERIES</div>
        <CardComponent
        :CardsList="CardListArray"/>
    
    </main>
</template>

<script>
import CardComponent from "./CardComponent.vue";
import CardArray from "../assets/data/CardArray"
export default {
name:'MainComponent',
components:{
    CardComponent,
},
data(){
    return{ 
        CardListArray:CardArray
    }
    },
}
</script>

<style lang="scss" scoped>
main{
    position: relative;
    background-color: black;
    .title{
        position: absolute;
        top:-20px;
        left: 100px;
        padding: 10px 15px;
        background-color: #0E88F9;
        color: white;
    }
}
</style>