<script>
	import illustration from 'images/illustration.svg';
</script>

<style lang="scss">
  @import 'breakpoint-sass/stylesheets/_breakpoint.scss';
  @import "../var.scss";
	#home {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		height: calc(100vh - 6rem);
		overflow: hidden;
		@include breakpoint($breakMobile) {
			height: calc(100vh - 10rem);
		}
	}
	.illustration {
		
		img {
			display: block;
			width: 100%;
			object-fit: cover;
		}
	}
	h1 {
		color: #192e3b;
		display: none;
		@include breakpoint($breakMobile) {
			font-size: 2rem;
			line-height: 2.4rem;
			margin-bottom: 1rem;
			display: block;
		}
	}
	h2 {
		@include breakpoint($breakMobile) {
			font-size: 1.4rem;
			line-height: 125%;
			max-width: none;
		}
	}
	h3 {
		font-size: 3rem;
		padding-left: 2rem;
		@include breakpoint($breakMobile) {
			font-size: 2rem;
			padding-left: 1.5rem;
		}
	}
</style>

<svelte:head>
	<title>FS Map Tool | See where you're flying on your tablet or phone.</title>
	<meta name="description" content="A mobile device map utility tool for MS Flight Simulator 2020 that lets you see your current airplane position on a map." />
</svelte:head>

<div id="home">
	<div class="text">
		<h1>FS Map Tool</h1>
		<h2 class="italic">A map utility tool for MS Flight Simulator 2020</h2>
		<h3 class="italic cite">See where you're flying on your tablet or phone.</h3>
	</div>
	<figure class="illustration">
		<img alt="FS Map Tool" src="{illustration}">
	</figure>
</div>