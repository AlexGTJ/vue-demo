<template>
    <h3>Key属性添加到v-for中</h3>
    <div v-for="(item,index) in names" :key="index">
        <p> {{ item }}</p>
    </div>
    <div v-for="(item,index) in results" :key="item.id">{{ item.name }}: {{ item.score }}</div>
</template>

<script>
export default {
    data(){
        return{
            names: ['张三', '李四', '王五'],
            results: [
                { name: '赵六', score: 100, id: 1},
                { name: '钱七', score: 90, id: 2},
                { name: '麻八', score: 80, id: 3},
            ],
        }
    }
}
</script>