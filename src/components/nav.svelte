<script>
  export let segment;
</script>

<style lang="scss">
  nav {
    display: flex;
    justify-content: space-between;
    flex-direction: row;
    align-items: center;
    background-color: #cae3e1;
    padding: 0 0 0 2rem;
  }
  ul {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    li {
      background-color: #4f9eaf;
      transition: background-color 250ms;
      &.active {
        background-color: #192e3b;
      }
      a {
        display: block;
        line-height: 4rem;
        color: white;
        padding: 0 2rem;
        text-decoration: none;
      }
    }
  }
</style>

<nav>
  <h1>FS Map Tool</h1>
  <ul>
    <li class:active={!segment}><a href=".">Home</a></li>
    <li class:active={segment === 'usage'}><a href="/usage">Usage</a></li>
    <li class:active={segment === 'support'}><a href="/support">Support</a></li>
  </ul>
</nav>