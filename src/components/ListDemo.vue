<template>
    <h3>列表渲染</h3>
    <ul>
        <li v-for="name in names" :key="name">{{ name }}</li>
    </ul>
    <ul>
        <li v-for="(result, index) in results" :key="index">
            {{ result.name }}: {{ result.score }}
        </li>
    </ul>
    <div>
        <p v-for="(result, index) in results" :key="index" :id="index">
            {{ result.name }}: {{ result.score }}
        </p>
        
    </div>

</template>
<script>
export default {
    data() {
        return {
            names: ['Alice', 'Bob', 'Cathy'],
            results: [
                { name: 'Alice', score: 100 },
                { name: 'Bob', score: 90 },
                { name: 'Cathy', score: 80 },
            ],
        }
    }
}
</script>