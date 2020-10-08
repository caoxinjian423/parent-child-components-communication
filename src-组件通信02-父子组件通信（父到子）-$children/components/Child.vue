<template>
    <div>
        <hr>
        <span>我是子组件</span>
        <br>
        这里子组件的title:{{title}}
    </div>
</template>

<script>
    export default {
        data() {
            return {
                title: "我是子组件的title！"
            }
        },
        methods: {
            setTitle() {
                this.title="更改后的子组件title！"
            }
        },
    }
</script>

<style scoped>

</style>