<template>
    <div>
        <hr>
        <span>我是子组件</span>
        <button @click="handleClick">点我更改父组件的msg</button>
    </div>
</template>

<script>
    export default {
        methods: {
            handleClick() {
                console.log(this.$parent.msg);
                this.$parent.setMsg("我是使用$parent更改的父级msg")
            }
        },
    }
</script>

<style scoped>

</style>