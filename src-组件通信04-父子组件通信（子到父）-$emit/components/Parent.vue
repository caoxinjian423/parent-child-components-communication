<template>
    <div>
        <span>我是父组件</span>
        <br>
        {{msg}}
        <Child :title="title" @child="handleMsg"></Child>
    </div>
</template>

<script>
    import Child from './Child';
    export default {
        components: {
            Child,
        }, 
        data() {
            return {
                title: "我是父组件传递的title！",
                msg: "我是父组件的msg"
            }
        },
        methods: {
            handleMsg(msg) {
                this.msg=msg;
            }
        },
    }
</script>

<style scoped>

</style>