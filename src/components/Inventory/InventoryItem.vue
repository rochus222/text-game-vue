<template>
  <div class="item">
    <a href="#">{{ title }}</a>
    <span class="icons">
      <font-awesome-icon class="icon" icon="plus" title="Take" aria-hidden="true" />
      <font-awesome-icon class="icon" icon="search" title="Look" aria-hidden="true" />
      <font-awesome-icon class="icon" icon="hammer" title="Combine" aria-hidden="true" />
    </span>
  </div>
</template>

<script>
export default {
  name: "InventoryItem",
  props: ["title", "active"]
};
</script>

<style scoped lang="less">
@import url("../../styles/variables.less");
a {
  text-decoration: none;
}

.icons {
  float: right;
}

.icon {
  margin-left: 10px;
}

.item {
  padding: 10px 2%;
  width: 96%;
  background: @dark-grey;
  color: @light-blue;
  border-bottom: 1px solid @light-blue;
}

.item:last-child {
  border-bottom: none;
}
</style>
