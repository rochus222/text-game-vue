<template>
  <div class="box">
    <div class="header">Game</div>
    <div
      class="body"
    >Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</div>
    <div class="footer">
      Go to:
      <a href="#">North</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Game"
};
</script>

<style scoped lang="less">
@import url("../../styles/variables.less");
.header {
  padding: 10px;
  width: 100%;
  font-size: 0.8em;
  color: @light-blue;
}
.body {
  padding: 10px;
  height: 200px;
  overflow-y: auto;
}
.footer {
  padding: 10px;
  color: @light-blue;
}
</style>
