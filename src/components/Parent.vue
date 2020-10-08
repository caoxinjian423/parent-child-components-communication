<template>
    <div>
        <span>我是父组件</span>
        <br>
        {{msg}}
        <Child ></Child>
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
            setMsg(msg) {
                this.msg=msg;
            }
        },
    }
</script>

<style scoped>

</style>