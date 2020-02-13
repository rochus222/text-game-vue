<template>
  <div class="box">
    <div class="body">
      <img src="@/assets/avatar.png" width="200px" height="200px" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Dialog"
};
</script>

<style scoped lang="less">
@import url("../../styles/variables.less");
.body {
  padding: 10px;
  height: 200px;
  text-align: center
}
</style>
