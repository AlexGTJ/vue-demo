<template>
    <h3>传递参数</h3>
    <button @click="addCount('hello vue')">点击我</button>
    <p>{{ count }}</p>
</template>

<script>
export default{
    data(){
        return{
            count:0
        }
    },
    methods:{
        addCount(msg){
            // console.log(e)
            // e.target.innerHTML = '点击了:'+this.count
            console.log(msg)
            this.count++
        }
    }
}

</script>