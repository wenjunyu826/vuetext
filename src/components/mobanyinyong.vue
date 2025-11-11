<template>
    <div class="mobanyinyong">
        <h3>模版引用</h3>
        <div class="container" ref="container">
            {{content}}
        </div>
        <button @click="changeContent">改变内容</button>
        <br>
        <input type="text" ref="username"></input>
    </div>
</template>

<script>
export default {
    name: 'mobanyinyong',
    data() {
        return {
            message: '这是模版引用的内容',
        }
    },
    methods: {
        changeContent() {
            console.log(this.$refs.container, "11111111111111111");
            this.$refs.container.innerHTML = '5555555555555555555';
            console.log(this.$refs.username.value, "2222222222222222222222");
        }
    }
}
</script>

<style scoped>
.mobanyinyong{
    color: yellow;
}
</style>