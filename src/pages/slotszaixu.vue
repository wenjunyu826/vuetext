<template>
    <h3>插槽3再续</h3>
    <slot name="herderer" :msg="childMsg"></slot>
    <slot name="mainin" :job="jobMsg"></slot>
</template>

<script>
export default {
  name: 'slotszaixu',
  data() {
    return {
      childMsg: '夏夏夏夏',
      jobMsg: '至至至至'
    }
  }
}
</script>