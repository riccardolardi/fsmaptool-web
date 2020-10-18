<script>
	import illustration from 'images/illustration.svg';
</script>

<style lang="scss">
	#home {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		height: calc(100vh - 10rem);
		overflow: hidden;
	}
	.illustration {
		display: flex;
		justify-content: center;
		
		img {
			display: block;
			width: 100%;
			object-fit: cover;
		}
	}
	h2, h3 {
		position: relative;
		z-index: 10;
		line-height: 150%;
	}
	h2 {
		color: #192e3b;
	}
	h3 {
		font-size: 3rem;
	}
</style>

<svelte:head>
	<title>FS Map Tool | See where you're flying on your tablet or phone.</title>
</svelte:head>

<div id="home">
	<div class="text">
		<h2 class="italic">A map utility tool for MS Flight Simulator 2020</h2>
		<h3 class="italic cite">See where you're flying on your tablet or phone.</h3>
	</div>
	<figure class="illustration">
		<img alt="FS Map Tool" src="{illustration}">
	</figure>
</div>