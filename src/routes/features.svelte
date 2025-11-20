<style lang="scss">
  @import 'breakpoint-sass/stylesheets/_breakpoint.scss';
  @import "../var.scss";
  #features {
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
    h3 {
      font-size: 1.4rem;
      font-style: italic;
      @include breakpoint($breakMobile) {
        font-size: 1.2rem;
      }
    }
    li {
      list-style: disc;
      margin-bottom: 0.5rem;
      @include breakpoint($breakMobile) {
        margin-bottom: 1rem;
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
            margin-bottom: 0.4rem;
            &:first-child {
              margin-top: 0.4rem;
            }
          }
        }
      }
    }
  }
</style>

<svelte:head>
  <title>FS Map Tool | Features</title>
  <meta name="description" content="Using FS Map Tool is easy. 1 + 1 = 2." />
</svelte:head>

<div id="features">
  <h2>Interactive Map, Waypoints, Flight Data,...</h2>
  <p class="italic">FS Map Tool is actively maintained and extended with new features on a regular basis.</p>
  <p>Currently these are the apps main features:</p>
  <ul>
    <li><h3>Interactive Map & plane location</h3>
      <ul>
        <li>Map can be dragged & zoomed like normal Google Maps / Apple Maps</li>
        <li>Switchable map types (satellite or plain)</li>
        <li>Plane icon can be changed (tap on plane to cycle)</li>
        <li>Toggle map center / auto-follow airplane</li>
        <li>Toggle lock view orientation to plane heading or to north</li>
      </ul>
    </li>
    <li><h3>Teleportation</h3>
      <ul>
        <li>Teleport your plane anywhere in the world in an instant</li>
        <li>Long-press on the location where you want to teleport</li>
        <li>A dialog will appear, select 'teleport'</li>
      </ul>
    </li>
    <li><h3>Custom Waypoints (no flight plan data import from FS 2020/2024 yet)</h3>
      <ul>
        <li>Add custom waypoints by long-pressing on a map location</li>
        <li>Move waypoints by long-pressing on a pin and dragging</li>
        <li>Remove waypoints by tapping on a pin and pressing the delete button</li>
        <li>Switch between active waypoints with top right waypoint control buttons</li>
      </ul>
    </li>
    <li><h3>Show additional flight parameters on a HUD, currently:</h3>
      <ul>
        <li>Heading, airspeed and altitude</li>
      </ul>
    </li>
  </ul>
</div>
