<template>
    <div>
        <span>我是父组件</span>
        <Child title="我是父组件传递的title"></Child>
    </div>
</template>

<script>
    import Child from './Child';
    export default {
        components: {
            Child,
        }, 
    }
</script>

<style scoped>

</style>