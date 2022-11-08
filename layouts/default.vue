<template>
  <div>
    <TheHeader @sidenavToggle="displaySidenav = !displaySidenav"/>
    <TheSidenav :show="displaySidenav" @close="displaySidenav=false"/>
    <Nuxt />
  </div>
</template>

<script>
import TheHeader from "../pages/navigation/TheHeader";
import TheSidenav from "../pages/navigation/TheSidenav";

export default {
  components: {
    TheHeader,
    TheSidenav,
  },
  data() {
    return {
      displaySidenav: false,
    };
  },
};
</script>

<style scoped>
html,
* {
  font-family: "Noto Sans", sans-serif, "Noto Serif", serif;
}

body {
  margin: 0;
  padding: 0;
}
</style>
