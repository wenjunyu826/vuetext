<template>
    <div class="yilaizhurusun">
        <h3>孙组件</h3>
        <p>我从父组件接收过来值：{{ title }}</p>
        <p>我从父组件接收过来消息：{{ msg }}</p>
        <p>{{ mess }}</p>
        <p>+++++++++{{ fullMess }}</p>
    </div>
</template>

<script>
export default {
    name: "yilaizhurusun",
    data() {
        return {
            fullMess: this.mess2
            
        }
    },
    props: {
        title: {
            type: String,
            default: '默认标题',
        },
        msg: {
            type: String,
            default: '默认消息',
        }
    },
    inject: ['mess2'],
}
</script>

<style scoped></style>