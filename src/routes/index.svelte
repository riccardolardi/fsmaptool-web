<script>
	import illustration from 'images/illustration.svg';
	import appstore from 'images/appstore.png';
	import googleplay from 'images/googleplay.png';
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
		position: relative;
		@include breakpoint($breakMobile) {
			height: calc(100vh - 10rem);
		}
	}
	.badges {
		display: flex;
		position: relative;
		top: 2rem;
		left: 2rem;
		@include breakpoint($breakMobile) {
			top: 1rem;
			left: 0px;
		}
	}
	.version-announcement {
		display: flex;
		justify-content: center;
		align-items: center;
		position: absolute;
		top: 6rem;
		right: 2vw;
		width: 16vmin;
		height: 16vmin;
		border-radius: 50%;
		background-color: #ee6161;
		transform: rotate(15deg);
		text-decoration: none;
		white-space: unset;
		@include breakpoint($breakMobile) {
			top: 2rem;
		}
		p {
			color: white;
			text-align: center;
			margin: 0;
			font-weight: bold;
			font-style: italic;
			font-size: 2.5vmin;
			line-height: 1.4;
		}
	}
	.appstore-badge,
	.googleplay-badge {
		height: 4vw;
		margin-right: 1rem;
		@include breakpoint($breakMobile) {
			height: 10vw;
		}
		a {
			display: block;
			height: 100%;
		}
		img {
			display: block;
			height: 100%;
		}
		&:last-child {
			margin-right: 0;
		}
	}
	.illustration {
		img {
			display: block;
			width: 100%;
		}
	}
	h1 {
		color: $greenDark;
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
		width: 80%;
		@include breakpoint($breakMobile) {
			font-size: 1.4rem;
			line-height: 125%;
		}
	}
	h3 {
		font-size: 3rem;
		padding-left: 2rem;
		width: 80%;
		@include breakpoint($breakMobile) {
			font-size: 1.5rem;
			line-height: 125%;
			padding-left: 0;
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
		<div class="badges">
			<figure class="appstore-badge">
				<a href="https://apps.apple.com/us/app/id1536321554#?platform=iphone" rel="noreferrer" target="_blank">
					<img alt="Download on the Apple App Store" src="{appstore}">
				</a>
			</figure>
			<figure class="googleplay-badge">
				<a href="https://play.google.com/store/apps/details?id=com.riccardolardi.fsmaptool" rel="noreferrer" target="_blank">
					<img alt="Download on Google Play" src="{googleplay}">
				</a>
			</figure>
		</div>
		<a href="/setup" class="version-announcement">
			<p>New Version 1.1.0</p>
		</a>
	</div>
	<figure class="illustration">
		<img alt="FS Map Tool" src="{illustration}">
	</figure>
</div>