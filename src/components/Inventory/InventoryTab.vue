<template>
  <a href="#" :class="{tab: true, active: active}">{{ title }}</a>
</template>

<script>
export default {
  name: "InventoryTab",
  props: [
      "title",
      "active"
  ]
};
</script>

<style scoped lang="less">
    @import url("../../styles/variables.less");
    .tab {
        padding: 10px;
        display: inline-block;
        border-top-right-radius: 5px;
        border-top-left-radius: 5px;
        margin-right: 5px;
        background: @blue;
        color: @dark-grey;
    }

    .active {
        color: @light-blue;
        background: @dark-blue;
    }
</style>
