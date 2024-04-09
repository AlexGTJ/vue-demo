<template>
    <h3>Hello World</h3>
    <p>{{ msg }}</p>
    <p>{{ num + 10 }}</p>
    <p>{{ result ? '真' : '假' }}</p>
    <p>{{ message.split("").reverse().join("") }}</p>
    <p v-html="rawHtml"></p>
    <p :id="id" :class="class">id: {{ id }}, class: {{ class }}</p>
    <button :disabled="isDisabled">按钮</button>
    <div v-bind="objectOfAttrs">v-bind</div>
</template>

<script>
export default {
    data(){
        return {
            msg: '你好 vue',
            num: 10,
            result: true,
            message: 'Hello Vue 3.0',
            rawHtml:'<a href="https://www.baidu.com">百度</a>',
            id: 1,
            class: 'myclass',
            isDisabled: false,
            objectOfAttrs:{
                id: 2,
                class: 'myclass',
            }
        }
    }
}
</script>

<style scoped>
.myclass {
    color: red;
    font-size: 15px;
}
</style>