<template>
  <div>
    <TheHeader @sidenavToggle="displaySideNav = !displaySideNav"/>
    <TheSidenav
      :show="displaySideNav" 
      @close="displaySideNav =!displaySideNav"
    />
    <nuxt />
  </div>
</template>

<script>
import TheHeader from '~/components/Navigation/TheHeader.vue'
import TheSidenav from '~/components/Navigation/TheSidenav.vue'

export default {
  components: {
    TheHeader,
    TheSidenav
  },
  data() {
    return {
      displaySideNav: false
    }
  }
}
</script>

<style>
  html {
    font-family: 'Open Sans', sans-serif;
  }
  body {
    margin: 0;
  }
</style>
