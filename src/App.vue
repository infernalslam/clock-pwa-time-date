<template>
  <div id="app">
      <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Noto+Sans');
body {
  margin: 0;
  background-color: #000;
}

#app {
  font-family: 'Noto Sans', sans-serif;s
  color: #2c3e50;
}

</style>
