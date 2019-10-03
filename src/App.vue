<template>
  <div id="app">
  <Header v-show = "$route.path === '/Login' || $route.path === '/Register'|| $route.path === '/' ? true: false"></Header>
  <AppBody></AppBody>
  <Sidebar v-show = "$route.path === '/Dashboard' || $route.path === '/Subjects'|| $route.path === '/PersonalInfo' ? true: false">
  </Sidebar>
  </div>
</template>

<style scoped lang="scss">
@import "assets/colors.scss";
#app{
  // background-image: $background-image !important;
  background-color: $tertiary;
  size: $size !important;
  background-repeat: $backgroud-repeat !important;
  overflow: $overflow !important;
  height: $height !important;
  max-height: $max-height !important;
}
</style>

<script>
import Sidebar from 'router/frame/Sidebar.vue'
import Header from 'router/frame/Header.vue'
import AppBody from 'router/frame/Body.vue'

export default {
  name: 'app',
  components: {
    Header,
    AppBody,
    Sidebar
  }
}



</script>
