<style lang="scss">
  @import 'breakpoint-sass/stylesheets/_breakpoint.scss';
  @import "../var.scss";
  #faq {
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
  <title>FS Map Tool | Frequently asked questions</title>
  <meta name="description" content="Find answers to the most Frequently asked questions." />
</svelte:head>

<div id="faq">
  <h2>Frequently asked questions.</h2>
  <p class="italic">If you face any issues, check here for possible solutions:</p>
  <ul>
    <li>Does this work on the XBox?
      <ul>
        <li>No, sadly this is only for the PC version currently.</li>
      </ul>
    </li>
    <li>I get an error saying "Uncaught Exception: Error: The specified module could not be found"
      <ul>
        <li>This means your system is lacking some Library files from Microsoft</li>
        <li>Namely the Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019</li>
        <li>You can download those files directly from Microsoft <a href="https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads" rel="noreferrer" target="_blank">here</a></li>
        <li>After installation of the redistributables the server should work as expected</li>
      </ul>
    </li>
    <li>I get an error saying "EADDRESS IN USE"
      <ul>
        <li>This means you have multiple instances of the server application running</li>
        <li>Kill all open instances using Windows Task Manager, then open it only once</li>
      </ul>
    </li>
    <li>The app keeps saying "Waiting for server data"
      <ul>
        <li>Ensure both your mobile device as well as your PC are on the same local network</li>
        <li>Confirm Windows firewall / security settings are not blocking the app communication</li>
        <li>Check your Wifi/LAN router settings, check router security options</li>
      </ul>
    </li>
    <li>I get a Windows warning saying the software might not be safe
      <ul>
        <li>This is false alarm and can be safely ignored</li>
      </ul>
    </li>
  </ul>
</div>
