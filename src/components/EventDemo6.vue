<template>
    <h3>事件修饰符</h3>
    <a href="https://cn.vuejs.org/guide/essentials/event-handling.html" @click.prevent="clickHandler">事件修饰符文档</a>
    <br/>
    <a href="https://cn.vuejs.org/guide/essentials/event-handling.html" @click="clickHandler">事件修饰符文档</a>
    <br/>
    <div @click="clickDiv">
        <p @click.stop="clickP">测试事件冒泡</p>
    </div>
</template>
<script>
export default{
    data(){
        return{

        }
    },
    methods:{
        clickHandler(){
            console.log('点击了')
        },
        clickDiv(){
            console.log('点击了div')
        },
        clickP(){
            console.log('点击了p')
        }
    }
}
</script>