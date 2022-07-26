<template>
  <div class="main">
    <div class="grid-container">
      <div class="grid-x grid-margin-x">
        <div class="cell large-6">
          <common-title class="margin-bottom-40" type="secondary">Fully Managed Cloud & Web Hosting</common-title>
          <div class="text">Deidcated resources, full root access, & easy scaling. It’s the virtual private server
            you’ve been cravin
          </div>
          <common-button color="light">View Pricing</common-button>
        </div>
        <div class="cell large-6">
          <div class="image"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CommonTitle from "@/components/common/Title";
import CommonButton from "@/components/common/Button";

export default {
  name: "IndexMain",
  components: {
    CommonTitle,
    CommonButton
  }
}
</script>

<style lang="scss" scoped>
@import "@/assets/scss/variables";

.main {
  padding: 350px 0;
  min-height: 100%;

  .text {
    margin-bottom: 40px;
    color: rgba($darkBlue, .5);
  }
}
</style>