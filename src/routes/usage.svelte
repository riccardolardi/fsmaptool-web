<script>
  
</script>

<style lang="scss">
  @import 'breakpoint-sass/stylesheets/_breakpoint.scss';
  @import "../var.scss";
  #usage {
    @include breakpoint($breakMobile) {
      padding-bottom: 15vh;
    }
  }
  ul {
    margin-top: 1rem;
    margin-left: 2rem;
    @include breakpoint($breakMobile) {
      margin-left: 1rem;
    }
    li {
      list-style: disc;
      @include breakpoint($breakMobile) {
        margin-bottom: 0.5rem;
      }
      ul {
        margin-top: 0;
        margin-left: 2rem;
        font-size: 1rem;
        line-height: 150%;
        @include breakpoint($breakMobile) {
          font-size: unset;
          line-height: unset;
          margin-left: 1rem;
        }
        li {
          list-style: circle;
          @include breakpoint($breakMobile) {
            margin-bottom: 0;
          }
        }
      }
    }
  }
</style>

<svelte:head>
  <title>FS Map Tool | How to use</title>
  <meta name="description" content="Using FS Map Tool is easy. 1 + 1 = 2." />
</svelte:head>

<div id="usage">
  <h2>Using FS Map Tool is easy.</h2>
  <p>You'll need the server app that acts as a gateway for communication between MS FS 2020 and FS Map Tool, and the client FS Map Tool mobile app.</p>
  <p>Follow these steps:</p>
  <ul>
    <li>Download the server app installer: <a href="/">FS Map Tool Server</a>
      <ul>
        <li>currently Windows 10 64bit only</li>
      </ul>
    </li>
    <li>Launch the installer, the app will install and launch automatically
      <ul>
        <li>The app will run in background and show up in the system tray as a small icon</li>
        <li>Clicking on the system tray app icon opens up a context menu</li>
        <li>The app will now listen for MS FS 2020 data and forward if requested</li>
      </ul>
    </li>
    <li>Click on the system tray app icon to show your PC IP address</li>
    <li>Download the mobile app from <a href="/">Apple App Store</a>
      <ul>
        <li>Android version / Google Play coming soon</li>
      </ul>
    </li>
    <li>Launch the mobile app on your mobile device and enter the PC IP address</li>
    <li class="italic">Ready to fly!</li>
  </ul>
</div>