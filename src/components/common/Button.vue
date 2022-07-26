<template>
  <a class="button" :class="[color, size]" :href="href" :target="target">
    <slot>Botão</slot>
  </a>
</template>

<script>
export default {
  name: "CommonButton",
  props: {
    color: {
      default: 'light',
      type: String
    },
    size: {
      default: 'regular',
      type: String
    },
    href: {
      default: null,
      type: String
    },
    target: {
      default: null,
      type: String
    }
  }
}
</script>

<style lang="scss" scoped>
@import "@/assets/scss/variables";

.button {
  display: inline-block;
  border-radius: 5px;
  color: #fff;
  font-size: 18px;

  &.light {
    background: $lightBlue;
  }

  &.dark {
    background: $darkBlue;
  }

  &.regular {
    padding: 10px 35px;
  }

  &.large {
    padding: 17px 38px;
  }
}
</style>