<template>
<div class="sort">
    <div v-for="(Item, index) in ITEM" :key="`Item_${index}`" >
        <h1 style="font-size: 3em">{{ Item.SORT }}</h1>
        <h3>针对{{ Item.SORT }}的项目练习</h3>
        <div class="item" v-for="(item, index) in Item.DEMO" :key="`item_${index}`" >
            <div class="item-img">
                <a :href="item.src" target="_black"><img :src="item.img" alt=""></a>
            </div>
            <div class="item-name">
                <h1><a :href="item.src" target="_black">{{ item.name }}</a></h1>
                <p>{{ item.describe }}</p>
            </div>
        </div>
    </div>
</div>

</template>
<script>
import Item from "../data/items"
export default {
    data(){
        return {
            ITEM: Item
        }
    }
};
</script>
<style lang="scss">
.sort{
    >div{
        margin: 10px 0 30px 0;
    }
    h1{
        text-align: center;
    }
    h3{
        display: block;
        margin: 0 30px;
    }
    .item{
        border: 1px solid #ccc;
        margin: 20px;
        padding: 10px 10px;
        display: inline-block;
        width: 370px;
        height: 100%;
        .item-img img{
            width: 100%;
        }
        .item-name{
            h1{
                margin: 15px;
            }
        }
    }
}

</style>