<template>
  <div>
    <TheHeader @sidenavToggle="displaySidnav = !displaySidnav"/>
    <TheSidenav @close="displaySidnav = false" :show="displaySidnav"/>
    <nuxt/>
  </div>
</template>

<script>
import TheHeader from "@/components/Navigation/TheHeader";
import TheSidenav from "@/components/Navigation/TheSideNav";
export default {
  components: {
    TheHeader,
    TheSidenav
  },
  data() {
    return {
      displaySidnav: false
    };
  }
};
</script>


<style>
html {
  font-family: "Open Sans", sans-serif;
}
body {
  margin: 0;
}
</style>
