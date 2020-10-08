<template>
    <div>
        <span>我是父组件</span>
        <Child></Child>
    </div>
</template>

<script>
    import Child from './Child';
    export default {
        components: {
            Child,
        }, 
        mounted () {
            console.log(this.$children[0].title);
            this.$children[0].setTitle();
        },
    }
</script>

<style scoped>

</style>