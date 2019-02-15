<template>
<div>
    <h2>goods_list商品列表</h2>
    <ul>
        <li :key="item.name" v-for="item of list">
            <nuxt-link :to="'/detail/' + item.id" >{{item.name}}</nuxt-link>
        </li>
    </ul>
</div>
</template>

<script>
export default {
    data(){
        return{
            list:[
                {id:'001',name:'iponexxx',price:2000},
                {id:'002',name:'mixx',price:4000},
                {id:'003',name:'huaweixxx',price:1000}
            ]
        }
    }
}
</script>
