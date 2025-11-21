<script>
  import GoogleAnalytics from "sapper-google-analytics/GoogleAnalytics.svelte";
  import { stores } from "@sapper/app";
  import Nav from "../components/nav.svelte";
  import Footer from "../components/footer.svelte";

  let ga_measurment_id = "UA-16856648-9";
  export let segment;
</script>

<GoogleAnalytics {stores} id={ga_measurment_id} />

<Nav {segment} />

<main>
  <slot></slot>
</main>

<Footer />

<style global lang="scss">
  @import "breakpoint-sass/stylesheets/_breakpoint.scss";
  @import "../var.scss";
  @import "../type.scss";
  #sapper {
    position: relative;
    min-height: 100vh;
  }
  main {
    padding: 2rem 2rem 0;
  }
  a {
    color: #192e3b;
    white-space: nowrap;
  }
</style>
