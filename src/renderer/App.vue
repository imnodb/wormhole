<template>
  <div id="app">
    <router-view></router-view>
    <div @click="startChrome">打开浏览器</div>
  </div>
</template>

<script>
// import path from 'path';
// import { remote } from 'electron';
// import startChrome from 'start-chrome';

export default {
  name: 'wormhole',
  methods: {
    startChrome() {
      global.alert(this.$electron.remote.app.getPath('userData'));
      // startChrome('');
    },
  },
};
</script>

<style>
/* CSS */
</style>
