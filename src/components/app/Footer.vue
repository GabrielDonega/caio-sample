<template>
  <footer>
    <div class="upper">
      <div class="grid-container">
        <div class="grid-x grid-margin-x">
          <div class="cell large-4">
            <div class="about">
              <div class="logo"/>
              <div class="text">Nulla diam felis, malesuada ut erat quis, mattis dignissim justo. Cras cursus, lacus et
                dignissim volutpat
              </div>
            </div>
          </div>
          <div class="cell large-8">
            <div class="grid-x grid-margin-x">
              <div class="cell large-4">
                <div class="menu-group">
                  <div class="title">Quick Links</div>
                  <ul>
                    <li>
                      <a href="#">Home</a>
                    </li>
                    <li>
                      <a href="#">About Us</a>
                    </li>
                    <li>
                      <a href="#">Services</a>
                    </li>
                    <li>
                      <a href="#">Contact Us</a>
                    </li>
                  </ul>
                </div>
              </div>
              <div class="cell large-4">
                <div class="menu-group">
                  <div class="title">Quick Links</div>
                  <ul>
                    <li>
                      <a href="#">Home</a>
                    </li>
                    <li>
                      <a href="#">About Us</a>
                    </li>
                    <li>
                      <a href="#">Services</a>
                    </li>
                    <li>
                      <a href="#">Contact Us</a>
                    </li>
                  </ul>
                </div>
              </div>
              <div class="cell large-4">
                <div class="menu-group">
                  <div class="title">Contact Us</div>
                  <ul>
                    <li>shield.info@gmail.com</li>
                    <li>+91 - 99xxx 000xx</li>
                  </ul>
                </div>
                <div class="menu-group">
                  <div class="title">Follow Us</div>
                  <ul>
                    <li>
                      <a href="#">Home</a>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="sub">
      <div class="grid-container">
        <div class="left">&copy; Copyright &copy; Sheild. All Rights Reserved.</div>
        <div class="right">
          <ul>
            <li>
              <a href="#">Privacy Policy</a>
            </li>
            <li>
              <a href="#">Tearms Condition</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter"
}
</script>

<style lang="scss" scoped>
@import "@/assets/scss/variables";

footer {
  color: $darkBlue;

  .upper {
    background: $lightGray;
    padding: 100px 0;

    .about {
      .logo {
        background: $darkBlue;
        margin-bottom: 40px;
        width: 195px;
        height: 50px;
      }

      .text {
        color: rgba($darkBlue, .5);
      }
    }

    .menu-group {
      .title {
        margin-bottom: 20px;
        color: #000;
        font-family: $ubuntu;
        font-weight: 700;
      }

      ul {
        li {
          color: rgba($darkBlue, .5);

          a {
            color: rgba($darkBlue, .5);
            transition: .4s;

            &:hover {
              color: $darkBlue;
            }
          }

          &:not(:last-child) {
            margin-bottom: 14px;
          }
        }
      }

      &:not(:last-child) {
        margin-bottom: 30px;
      }
    }
  }

  .sub {
    padding: 40px 0;
    font-size: 13px;

    .grid-container {
      display: flex;
      align-items: center;

      .left {
      }

      .right {
        margin-left: auto;

        ul {
          display: flex;
          align-items: center;

          li {
            a {
              color: $darkBlue;

              &:hover {
                text-decoration: underline;
              }
            }

            &:not(:last-child) {
              &:after {
                display: inline-block;
                content: '|';
                padding: 0 10px;
              }
            }
          }
        }
      }
    }
  }
}
</style>