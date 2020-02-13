<template>
  <div id="app">
    <Game />
    <Inventory />
    <Dialog />
    <Avatar />
  </div>
</template>

<script>
import Game from './components/Game';
import Inventory from './components/Inventory';
import Dialog from './components/Dialog';
import Avatar from './components/Avatar'

export default {
  name: "app",
  components: {
    Game,
    Inventory,
    Dialog,
    Avatar
  }
};
</script>

<style lang="less">
@import url('./styles/variables.less');

body {
  background: @blue;
  color: @white;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  width: 100%;
  max-width: 800px;
  margin: 60px auto;
}

.box {
  position: relative;
  border-radius: 5px;
  background: @dark-grey;
  width: 100%;
  margin-bottom: 5px;
  width: 100%;
  display: block;
  float: left;
}

.box:nth-child(2n+1) {
  width: 59%;
  margin-right: 1%;
}

.box:nth-child(2n) {
  width: 40%;
}

a, a:hover {
  color: inherit;
  font-weight: 900;
}
</style>
