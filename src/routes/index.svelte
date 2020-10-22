<script>
	import illustration from 'images/illustration.svg';
	import appstore from 'images/appstore.png';
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
	.appstore-badge {
		position: relative;
		top: 2rem;
		left: 2rem;
		width: 15vw;
		max-width: 256px;
		@include breakpoint($breakMobile) {
			top: 1rem;
			left: 1.5rem;
			width: 33.333vw;
		}
		a {
			display: block;
		}
		img {
			display: block;
			width: 100%;
			object-fit: cover;
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
		margin-bottom: 1rem;
		@include breakpoint($breakMobile) {
			font-size: 1.4rem;
			line-height: 125%;
		}
	}
	h3 {
		font-size: 3rem;
		padding-left: 2rem;
		@include breakpoint($breakMobile) {
			font-size: 1.75rem;
			line-height: 125%;
			padding-left: 1.5rem;
		}
	}
</style>

<svelte:head>
	<title>FS Map Tool | Transform your tablet or phone into an external map display.</title>
	<meta name="description" content="A mobile device (iOS and Android) map utility tool for Microsoft Flight Simulator 2020 that lets you see your current airplane position on an interactive map." />
</svelte:head>

<div id="home">
	<div class="text">
		<h1 class="bold">FS Map Tool</h1>
		<h2 class="italic">A map utility tool for Microsoft Flight Simulator 2020</h2>
		<h3 class="italic cite">See where you're flying on your tablet or phone.</h3>
		<figure class="appstore-badge">
			<a href="https://apps.apple.com/us/app/id1536321554#?platform=iphone" rel="noreferrer" target="_blank">
				<img alt="Download on the Apple App Store" src="{appstore}">
			</a>
		</figure>
	</div>
	<figure class="illustration">
		<img alt="FS Map Tool" src="{illustration}">
	</figure>
</div>