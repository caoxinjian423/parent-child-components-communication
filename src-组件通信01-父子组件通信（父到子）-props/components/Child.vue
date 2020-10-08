<template>
    <div>
        <hr>
        <span>我是子组件</span>
        <br>
        这里显示父组件传递的title:{{title}}
    </div>
</template>

<script>
    export default {
        props:["title"]
    }
</script>

<style scoped>

</style>