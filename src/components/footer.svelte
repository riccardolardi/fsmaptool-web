<script>

</script>

<style lang="scss">
  @import 'breakpoint-sass/stylesheets/_breakpoint.scss';
  @import "../var.scss";
  footer {
    display: flex;
    justify-content: space-between;
    position: absolute;
    width: 100%;
    bottom: 0px;
    background-color: #192e3b;
    padding: 1rem;
  }
  ul {
    display: flex;
    & + ul {
      li {
        &:last-child {
          &:after {
            content: "";
          }
        }
      }
    }
  }
  .left {
    display: flex;
    flex-wrap: wrap;
    font-size: 0.85rem;
    @include breakpoint($breakMobile) {
      font-size: 3vw;
    }
    li {
      margin-right: 1rem;
      @include breakpoint($breakMobile) {
        margin-right: 0.25rem;
      }
      &:after {
        content: "|";
        margin-left: 1rem;
        @include breakpoint($breakMobile) {
          margin-left: 0.25rem;
        }
      }
      a {
        color: white;
      }
    }
  }
</style>

<footer>
  <div class="left">
    <ul>
      <li><a href="https://apps.apple.com/us/app/id1536321554#?platform=iphone" rel="noreferrer" target="_blank">Apple App Store</a></li>
      <li><a href="https://play.google.com/store/apps/details?id=com.riccardolardi.fsmaptool" rel="noreferrer" target="_blank">Google Play</a></li>
      <li><a href="https://github.com/riccardolardi/fsmaptool-client" rel="noreferrer" target="_blank">Github Client</a></li>
    </ul>
    <ul>
      <li><a href="https://github.com/riccardolardi/fsmaptool-server" rel="noreferrer" target="_blank">Github Server</a></li>
      <li><a href="https://github.com/riccardolardi/fsmaptool-web/blob/master/PRIVACY.md" rel="noreferrer" target="_blank">Privacy Policy</a></li>
      <li><a href="https://github.com/riccardolardi/fsmaptool-web/blob/master/TERMS.md" rel="noreferrer" target="_blank">Terms of use</a></li>
    </ul>
  </div>
  <ul class="right">
    <li>
      <span class="italic">Happy Flying!</span>
    </li>
  </ul>
</footer>