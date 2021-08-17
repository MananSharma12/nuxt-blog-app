<template>
  <div>
     <TheHeader @sidenavToggle="displaySidenav = !displaySidenav" />
     <TheSidenav :show="displaySidenav" @close="displaySidenav = false" />
    <Nuxt />
  </div>
</template>

<script>
import TheHeader from '@/components/Navigation/TheHeader'
import TheSidenav from '@/components/Navigation/TheSidenav'

export default {
  data() {
    return {
      displaySidenav: false
    }
  },
  components: {
    TheHeader, 
    TheSidenav
  }
}
</script>

<style>
html{
    font-family: 'Open Sans', sans-serif;
}
body{
    margin: 0;
}
</style>