<template>
    <h3>事件传递参数</h3>
    <p @click="getNameHandler(name,$event)" v-for="(name,index) in names" :key="index">{{ name }}</p>
</template>
<script>
export default {
    data(){
        return{
            names:['张三','李四','王五']
        }
    },
    methods:{
        getNameHandler(name,e){
            console.log(name)
            console.log(e)
        }
    }
}
</script>