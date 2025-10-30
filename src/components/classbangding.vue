<template>
    <div class="classbangding">
        <h3>class动态绑定</h3>
        <p :class="myclass">1111111111</p>
        <h5>动态绑定对象示例</h5>
        <p :class="{'active': isActive, 'text-danger': hasError}">class绑定样式1</p>
        <p :class="classObject">class绑定样式2</p>
        <h5>动态绑定数组示例</h5>
        <p :class="[arrActive, arrHasError]">class绑定样式3</p>
        <p :class="[isActive ? 'active' : '']">class绑定样式4</p>
        <p :class="[isActive ? 'active' : '', { 'text-danger' :hasError}]">class绑定样式5</p>
    </div>
</template>

<script>
export default {
    name: 'classbangding',
    data() {
        return {
            myclass:'demo',
            isActive: true,
            hasError: true,
            classObject:{
                'active': true,
                'text-danger': true
            },
            arrActive:'active',
            arrHasError:'text-danger'
        };
    },
}
</script>

<style scoped>
.classbangding{
    color: slateblue;    
}
.active{
    font-size: 35px;
}
.text-danger{
    color: red;
}
</style>