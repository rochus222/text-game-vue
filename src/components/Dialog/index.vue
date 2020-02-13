<template>
  <div class="box">
    <div class="body">
      <div class="dialog-bubble">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
      </div>
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
  height: 220px;
  background: @blue;
  z-index: 100;
}

.dialog-bubble {
  padding: 10px 2%;
  width: 90%;
  height: 200px;
  overflow-y: auto; 
  background: @dark-grey;
  border-radius: 5px;
}

.dialog-bubble p {
  margin: 0;
  z-index: 10;
  position: relative;
}

.dialog-bubble::before {
  content: " ";
  width: 5%;
  padding-bottom: 5%;
  background: @dark-grey;
  position: absolute;
  bottom: 80px;
  right: 20px;
  transform: rotate(45deg);
}
</style>
