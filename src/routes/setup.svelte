<style lang="scss">
  @import 'breakpoint-sass/stylesheets/_breakpoint.scss';
  @import "../var.scss";
  #setup {
    padding-bottom: 6rem;
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
      margin-bottom: 0.5rem;
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
          margin-bottom: 0;
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

<div id="setup">
  <h2>Using FS Map Tool is easy.</h2>
  <p class="italic">Alongside the mobile app you'll need to install the server application on your PC, which will act as a gateway for communication between MS FS 2020/2024 and FS Map Tool.</p>
  <p>Follow these steps:</p>
  <ul>
    <li>Download the server app installer (currently Windows 10 64bit only)
      <ul>
        <li><a href="https://fsmaptool.riccardolardi.com/1.1.0/FS Map Tool Server Setup 1.1.0.exe">FS Map Tool Server Setup 1.1.0</a></li>
      </ul>
    </li>
    <li>Launch the installer, the app will install and launch automatically
      <ul>
        <li>The app will run in background and show up in the system tray as a small icon</li>
        <li>Clicking on the system tray app icon opens up a context menu</li>
        <li>The app will now listen for MS FS 2020/2024 data and forward if requested</li>
        <li>The tray icon will turn to green as soon as it's connected with MS FS 2020/2024</li>
      </ul>
    </li>
    <li>Click on the system tray app icon to show your PC IP address</li>
    <li>Download the mobile app for your tablet or phone
      <ul>
        <li><a href="https://apps.apple.com/us/app/id1536321554#?platform=iphone" rel="noreferrer" target="_blank"><b>iOS</b> FS Map Tool on Apple App Store</a></li>
        <li><a href="https://play.google.com/store/apps/details?id=com.riccardolardi.fsmaptool" rel="noreferrer" target="_blank"><b>Android</b> FS Map Tool on Google Play Store</a></li>
      </ul>
    </li>
    <li>Launch the mobile app on your mobile device and enter the PC IP address</li>
    <li class="italic">Ready to fly!</li>
  </ul>
</div>
