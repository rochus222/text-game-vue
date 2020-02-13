<template>
  <div class="box">
    <div class="header">
      <InventoryTab title="Items" :active="true"/>
      <InventoryTab title="Inventory"/>
    </div>
    <div class="body">
      <InventoryItem title="Item 1" />
      <InventoryItem title="Item 2" />
      <InventoryItem title="Item 3" />
      <InventoryItem title="Item 4" />
      <InventoryItem title="Item 5" />
      <InventoryItem title="Item 6" />
      <InventoryItem title="Item 7" />
      <InventoryItem title="Item 8" />
      <InventoryItem title="Item 9" />
      <InventoryItem title="Item 10" />
    </div>
  </div>
</template>

<script>
import InventoryTab from "./InventoryTab";
import InventoryItem from "./InventoryItem";

export default {
  components: {
    InventoryTab,
    InventoryItem
  },
  name: "Game"
};
</script>

<style scoped lang="less">
@import url("../../styles/variables.less");
a {
  text-decoration: none;
}

.header {
  width: 100%;
  font-size: 1.2em;
  color: @light-blue;
  margin-bottom: 5px;
  background: @blue;
}
.body {
  height: 245px;
  width: 100%;
  position: relative;
  display: block;
  overflow-y: auto;
  border-radius: 5px;
}
</style>
