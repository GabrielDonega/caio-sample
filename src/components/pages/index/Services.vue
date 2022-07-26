<template>
  <div class="services">
    <div class="grid-container">
      <div class="cell text-center">
        <common-title class="margin-bottom-50" type="secondary"/>
      </div>
      <div class="cell">
        <div class="items grid-x grid-margin-x">
          <div v-for="i in 6" class="item cell large-4 medium-6 small-12" :key="i">
            <div class="icon"></div>
            <div class="title">Shared Web Hosting</div>
            <div class="description">Vestibulum tristique urna eget odio interdum pellentesque. In sodales venenatis
              lectus, ac tincidunt quam placerat egestas.
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CommonTitle from '@/components/common/Title'

export default {
  name: "IndexServices",
  components: {
    CommonTitle
  }
}
</script>

<style lang="scss" scoped>
@import "@/assets/scss/variables";

.services {
  padding: 100px 0;
  background: $lightGray;

  .items {
    .item {
      display: flex;
      text-align: center;
      flex-direction: column;
      align-items: center;

      .icon {
        background: #fff;
        margin-bottom: 30px;
        width: 100px;
        height: 100px;
      }

      .title {
        margin-bottom: 25px;
        color: $darkBlue;
        font-size: 20px;
        font-weight: 700;
      }

      .description {
        color: rgba($darkBlue, .5);
      }

      &:not(:last-child) {
        margin-bottom: 80px;
      }
    }
  }
}
</style>