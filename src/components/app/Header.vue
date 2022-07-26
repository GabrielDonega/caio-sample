<template>
  <header>
    <div class="grid-container">
      <div class="content">
        <div class="left">
          <div class="logo"/>
        </div>
        <div class="right">
          <ul class="menu">
            <li>
              <a href="">Home</a>
            </li>
            <li>
              <a href="">About Us</a>
            </li>
            <li>
              <a href="">Services</a>
            </li>
            <li>
              <a href="">Contact Us</a>
            </li>
            <li>
              <common-button href="https://google.com" size="large" target="_blank">Login</common-button>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import CommonButton from "@/components/common/Button";

export default {
  name: "AppHeader",
  components: {
    CommonButton
  }
}
</script>

<style lang="scss" scoped>
@import "../../assets/scss/variables";

header {
  position: fixed;
  top: 0;
  left: 0;
  padding: 40px 0;
  width: 100%;

  .content {
    display: flex;
    align-items: center;

    .left {
      .logo {
        background: $darkBlue;
        width: 195px;
        height: 50px;
      }
    }

    .right {
      margin-left: auto;

      .menu {
        display: flex;
        align-items: center;

        li {
          a {
            font-size: 18px;
            font-weight: 500;
          }

          &:not(:last-child) {
            margin-right: 40px;

            a {
              color: $darkBlue;
            }
          }
        }
      }
    }
  }
}
</style>