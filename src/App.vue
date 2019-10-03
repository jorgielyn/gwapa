<template>
  <div id="app">
  <Header></Header>
  <AppBody></AppBody>
  <!-- <Sidebar v-show = "$route.path === '/Dashboard' || $route.path === '/Subjects'|| $route.path === '/PersonalInfo' ? true: false">
  </Sidebar> -->
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
// import Sidebar from 'components/frame/Sidebar.vue'
import Header from 'components/frame/Header.vue'
import AppBody from 'components/frame/Body.vue'

export default {
  name: 'app',
  components: {
    Header,
    AppBody
    
  }
}



</script>
