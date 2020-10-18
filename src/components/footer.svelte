<script>

</script>

<style lang="scss">
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
    &.left {
      font-size: 0.85rem;
    }
    &.right {
      
    }
    li {
      margin-right: 1rem;
      &:after {
        content: "|";
        margin-left: 1rem;
      }
      &:last-child {
        margin-right: 0;
        &:after {
          content: "";
        }
      }
      a {
        color: white;
      }
    }
  }
</style>

<footer>
  <ul class="left">
    <li><a href="">Apple App Store</a></li>
    <li><a href="">Google Play</a></li>
    <li><a href="https://github.com/riccardolardi/fsmaptool-client">Github Client</a></li>
    <li><a href="https://github.com/riccardolardi/fsmaptool-server">Github Server</a></li>
    <li><a href="https://github.com/riccardolardi/fsmaptool-web/blob/master/PRIVACY.md">Privacy Policy</a></li>
    <li><a href="https://github.com/riccardolardi/fsmaptool-web/blob/master/TERMS.md">Terms of use</a></li>
  </ul>
  <ul class="right">
    <li>
      <span class="italic">Happy Flying!</span>
    </li>
  </ul>
</footer>