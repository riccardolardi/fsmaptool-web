<script>
  
</script>

<style lang="scss">
  @import 'breakpoint-sass/stylesheets/_breakpoint.scss';
  @import "../var.scss";
  #support {
    @include breakpoint($breakMobile) {
      padding-bottom: 15vh;
    }
  }
</style>

<svelte:head>
  <title>FS Map Tool | Get in touch</title>
  <meta name="description" content="Get in touch with the developer." />
</svelte:head>

<div id="support">
  <h2>Let me know what you think.</h2>
  <p>This software has been made in my spare time as a fun side project. Still, I'm committed to keep up with development, listen to feedback, add new features and fix bugs.</p>
  <p>You can reach me at <a href="mailto:hello@riccardolardi.com">hello@riccardolardi.com</a></p>
  <p>The software is open source and the entire code can be viewed and built from scratch from Github (see links in footer below).</p>
  <p>Nonetheless I ask for a symbolic $1 for the mobile app. Despite being a side project a lot of effort has gone into the design, accessibility and user friendliness of this product. <u>Thanks for your understanding</u>.</p>
</div>