<template>
    <div class="shijianchuancan">
        <h3>事件传参</h3>
        <button @click="count1">add 454</button>
        <p>count is {{ countNum }}</p>
    </div>

</template>

<script>
export default {
    name: 'shijianchuancan',
    data() {
        return {
            countNum:0
        }
    },
    methods: {
        count1(e) {
            console.log(e, '4545445456565656565');
            console.log(e.targete,'e.targete.targete.targete.targete');
            console.log(e.currentTarget, 'e.currentTarget.currentTarget.currentTarget');
            console.log(e.target.innerHTML,'e.target.innerHTML.e.target.innerHTML.e.target.innerHTML');
            e.target.innerHTML = "添加添加" + this.countNum;
            this.countNum += 454;
        },
        newCount(msg) {
            console.log(msg, 'msgmsgmsgmsg')
        }
    }
}

</script>

<style scoped>
.shijianchuancan{
    color: royalblue;
}
</style>