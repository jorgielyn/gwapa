<template>
<div>
  <sidebar-menu :menu="menu" id="menu"/>
</div>
</template>
 
<style scoped lang="scss">
@import "assets/colors.scss";
  #menu{
    height: 94%;
    margin-top: 4%;  }
</style>

<script>
export default {
  name:'side',
  data() {
    return {
      menu: [
        {
          header: true,
          title: 'Main Navigation',
          hiddenOnCollapse: true
        },
        {
          href: '/Dashboard',
          title: 'Dashboard',
          icon: 'fas fa-tachometer-alt'
        },
        {
          href: '/Subjects',
          title: 'Subjects',
          icon: 'fas fa-plus-square'
        },
        {
          href: '/PersonalInfo',
          title: 'Personal Info',
          icon: 'fas fa-user',

        },
        {
          href: '/Login',
          title: 'Logout',
          icon: 'fas fa-power-off'
        }
      ]
    };
  }
};
</script> 