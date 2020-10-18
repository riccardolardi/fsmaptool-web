<script>
	import Nav from '../components/nav.svelte';
	import Footer from '../components/footer.svelte';
	export let segment;
</script>

<style global lang="scss">
	@font-face {
	  font-family: 'Ubuntu';
	  font-weight: 400;
	  font-style: normal;
	  font-display: swap;
	  src: url('/fonts/Ubuntu-Regular.ttf');
	}
	@font-face {
	  font-family: 'Ubuntu-Italic';
	  font-weight: 400;
	  font-style: normal;
	  font-display: swap;
	  src: url('/fonts/Ubuntu-Italic.ttf');
	}
	@font-face {
	  font-family: 'Ubuntu-Bold';
	  font-weight: 400;
	  font-style: normal;
	  font-display: swap;
	  src: url('/fonts/Ubuntu-Bold.ttf');
	}
	#sapper {
		position: relative;
		min-height: 100vh;
	}
	body {
		font-family: 'Ubuntu';
		font-size: 1.6rem;
		line-height: 135%;
		color: #4f9eaf;
	}
	main {
		padding: 2rem;
	}
	a {
		color: #192e3b;
	}
  h1 {
    font-size: 2rem;
    line-height: 4rem;
  }
  .italic {
  	font-family: 'Ubuntu-Italic';
  }
  .cite {
		&:before {
			content: "«";
		}
		&:after {
			content: "»";
		}
  }
  p {
  	max-width: 65vw;
	  & + p {
	    margin-top: 1rem;
	  }
  }
</style>

<Nav {segment} />

<main>
	<slot></slot>
</main>

<Footer />