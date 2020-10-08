<template>
    <div>
        <hr>
        <span>我是子组件</span>
        <button @click="handleClick">点我更改父组件的msg</button>
        <br>
        这里是父组件传递的title:{{title}}
    </div>
</template>

<script>
    export default {
        props:["title"],
        methods: {
            handleClick() {
                this.$emit("child", "更改后的父级msg")
            }
        },
    }
</script>

<style scoped>

</style>