<template>
    <h3>方法事件处理器</h3>
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
        addCount(){
            console.log('点击了按钮')
            console.log(this.count)
            this.count++
        }
    }
}

</script>