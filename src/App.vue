<template>
  <app-header/>

  <index-main/>
  <index-services/>

  <app-footer/>
</template>

<script>
import AppHeader from "@/components/app/Header";
import AppFooter from "@/components/app/Footer";

import IndexMain from "@/components/pages/index/Main";
import IndexServices from "@/components/pages/index/Services";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
    IndexMain,
    IndexServices
  }
}
</script>

<style lang="scss">
@import "assets/scss/variables";
@import "assets/scss/foundation";
@import "assets/scss/fonts";
@import "assets/scss/reset";
@import "assets/scss/classes";

@include foundation-xy-grid-classes();

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500&family=Roboto:wght@500;700;900&family=Ubuntu:wght@700&display=swap');

body {
  font-family: $poppins;
}

#app {
  height: 100%;
}
</style>
