<template>
    <h3>条件渲染</h3>
    <div v-if="show">{{ show }}: 你看得见我</div>
    <div v-else>{{ show }}: 你看不见我</div>
    <div v-if="type === 'A'">A</div>
    <div v-else-if="type === 'B'">B</div>
    <div v-else-if="type === 'C'">C</div>
    <div v-else>Not A/B/C</div>
    <div v-show="show">v-show: 你看得见我</div>
</template>
<script>
export default {
    data() {
        return {
            show: false,
            type: 'B',
        }
    }
}
</script>