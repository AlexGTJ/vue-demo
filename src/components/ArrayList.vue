<template>
    <h3>数组变化侦听</h3>
    <input type="text" v-model="username" :key="username" />
    <button @click="addListHandler">添加数据</button>
    <ul>
        <li v-for="name in names" :key="name">{{name}}</li>
    </ul>
</template>
<script>
export default{
    data(){
        return{
            names:['张三','李四','王五']
        }
    },
    methods:{
        addListHandler(){
            this.names.push(this.username)
        }
    }

}
</script>