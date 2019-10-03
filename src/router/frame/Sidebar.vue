<template>
  <sidebar-menu :menu="menu"  id="menu"/>
</template>
 
<style scoped lang="scss">
@import "assets/colors.scss";
  #menu{
    margin-top: $margin-top1 !important
  }
</style>

<script>
export default {
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