<template>
    <ul>
        <li
        v-for="(iconItem , index ) in BannerList" :key="`menu-${index}`"
        >
            <a href="#">
                <img :src="iconItem.icon" :alt="iconItem.title">
                <span>{{iconItem.title}}</span>
            </a>
        </li>
    </ul>
</template>

<script>


export default {
name:'BannerFooter',
props:{
    BannerList:Array
}

}
</script>

<style lang="scss" scoped>
ul{
    display: flex;
    justify-content: space-evenly;
    list-style: none;
    height: 100%;
    align-items: center;
    align-content: center;
    a{
        display: flex;
        align-items: center;
        font-size: 0.8rem;
        img{
        width: 36px;
        padding-right: 5px;
        }
    }
}

</style>