<style lang="scss">
  @import 'breakpoint-sass/stylesheets/_breakpoint.scss';
  @import "../var.scss";
  #support {
    padding-bottom: 6rem;
    @include breakpoint($breakMobile) {
      padding-bottom: 15vh;
    }
    p + h2,
    h2 + p {
      margin-top: 1rem;
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
  <p>You can reach me at <a href="mailto:info@fsmaptool.com">info@fsmaptool.com</a></p>
  <p>The software is open source and the entire code can be viewed and built from scratch from Github (see links in footer below).</p>
  <p>Nonetheless I ask $3 for the mobile app. Despite being a side project a lot of effort has gone into the design, accessibility and user friendliness of this product. Thanks for your understanding.</p>
  <h2>Donations</h2>
  <p>You're welcome to donate if you appreciate the product and would like to support further development: <a href="https://www.paypal.com/donate?business=9EBEWQTA4A2KU&currency_code=CHF">Donate via Paypal</a> Thanks a lot!</p>
</div>