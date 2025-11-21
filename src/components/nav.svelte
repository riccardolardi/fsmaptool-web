<script>
  export let segment;
</script>

<nav>
  <h1 class="bold"><a href="/">FS Map Tool</a></h1>
  <ul>
    <li class:active={!segment}><a href=".">Home</a></li>
    <li class:active={segment === "features"}>
      <a href="/features">Features</a>
    </li>
    <li class:active={segment === "setup"}><a href="/setup">Setup</a></li>
    <li class:active={segment === "faq"}><a href="/faq">FAQ</a></li>
    <li class:active={segment === "support"}><a href="/support">Support</a></li>
  </ul>
</nav>

<style lang="scss">
  @import "breakpoint-sass/stylesheets/_breakpoint.scss";
  @import "../var.scss";
  nav {
    display: flex;
    justify-content: space-between;
    flex-direction: row;
    align-items: center;
    position: sticky;
    top: 0px;
    background-color: #cae3e1;
    padding: 0 0 0 2rem;
    @include breakpoint($breakMobile) {
      flex-direction: column-reverse;
      align-items: stretch;
      padding: 0;
    }
  }
  ul {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    li {
      background-color: $greenLight;
      transition: background-color 250ms;
      @include breakpoint($breakMobile) {
        flex: 1;
      }
      &.active {
        background-color: $greenDark;
      }
      a {
        display: block;
        line-height: 4rem;
        color: white;
        padding: 0 2rem;
        text-decoration: none;
        text-align: center;
        @include breakpoint($breakMobile) {
          padding: 0;
        }
      }
    }
  }
  h1 {
    @include breakpoint($breakMobile) {
      display: none;
    }
    a {
      color: unset;
      text-decoration: none;
    }
  }
</style>
