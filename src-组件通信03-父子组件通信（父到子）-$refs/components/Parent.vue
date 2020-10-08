<template>
    <div>
        <span>我是父组件</span>
        <Child ref="Child"></Child>
    </div>
</template>

<script>
    import Child from './Child';
    export default {
        components: {
            Child,
        }, 
        mounted () {
            console.log(this.$refs.Child.title);
            this.$refs.Child.setTitle();
        },
    }
</script>

<style scoped>

</style>