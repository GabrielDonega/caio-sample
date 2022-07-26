<template>
  <component :is="titleType" class="title" :class="[type, color]">
    <slot>Título</slot>
  </component>
</template>

<script>
export default {
  name: "CommonTitle",
  props: {
    type: {
      default: 'primary',
      type: String
    },
    color: {
      default: 'dark',
      type: String
    }
  },
  computed: {
    // eslint-disable-next-line vue/return-in-computed-property
    titleType() {
      switch (this.type) {
        case 'primary':
          return 'h1'
        case 'secondary':
          return 'h2'
      }
    }
  }
}
</script>

<style lang="scss" scoped>
@import "@/assets/scss/variables";

.title {
  &.secondary {
    font-size: 40px
  }

  &.dark {
    color: $darkBlue;
  }

  &.light {
    color: $lightBlue
  }
}
</style>