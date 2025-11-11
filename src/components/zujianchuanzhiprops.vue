<template> 
<div class="zujianchuanzhiprops">
    <hr>
    <h3>组件传值(父传子)props</h3>
    <Child :message="message" :age="age" :name="name" :userInfo="userInfo"></Child>
</div>
</template>

<script>
import Child from '../pages/child.vue';
export default {
    name: 'zujianchuanzhiprops',
    data() {
        return {
            message: '父组件传值给子组件',
            age: 18,
            name:['张三','李四','王五'],
            userInfo:{
                title:'78997879879',
                id:'123'
            }
        }
    },
    components: {
        Child
    }
}
</script>

<style scoped>
.zujianchuanzhiprops {
    color: yellow;
}
</style>
