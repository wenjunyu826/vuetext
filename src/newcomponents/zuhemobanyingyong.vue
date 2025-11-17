<template>
    <div class="zuhemobanyingyong">
        <h3>组合式---模版引用</h3>
        <p ref="message">这是组合式模版引用的内容</p>
        <hr>
    </div>
</template>

<script setup>
import { ref, onMounted, watch } from 'vue';

const message = ref(null);

onMounted(() => {
    message.value.style.color = 'Aqua';
    message.value.style.fontSize = '30px';
    message.value.innerHTML = '+++++6666655656565++++';
});
</script>

<style scoped>
.zuhemobanyingyong{
    color: red;
}
</style>