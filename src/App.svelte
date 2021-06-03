<script>
	export let name;
	export let videoSrc;
</script>

<main>
	<h1>Hello {name}!</h1>
	<video controls src={videoSrc} data-path="">
	<script src="https://cdn.jsdelivr.net/npm/@webtor/player-sdk-js/dist/index.min.js" charset="utf-8" async></script>
	<track kind="captions">
	</video>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>