<template>
    <h3>事件参数</h3>
    <button @click="addCount">点击我</button>
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
        addCount(e){
            console.log(e)
            e.target.innerHTML = '点击了:'+this.count
            this.count++
        }
    }
}

</script>