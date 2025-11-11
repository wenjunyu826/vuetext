<template>
    <div class="child">
        <h3>child</h3>
        <p>{{ message }}</p>
        <p>{{ age }}</p>
        <p v-for="(item, index) in name" :key="index">{{ item }}</p>
        <p>{{ userInfo.title }}</p>
        <p>{{ userInfo.id }}</p>
    </div>
</template>

<script>
export default {
    name: 'child',
    data() {
        return {};
    },
    props: ["message", "age","name","userInfo"],
}
</script>

<style scoped>
.child {
    color: blue;
}
</style>
