<script lang="ts">
	document.addEventListener('mousemove', (ev) => {
		const cat = document.getElementById("goodboy");

		const yOffset = 0;
		const xOffset = 100;
	    const left = ev.pageX + xOffset;
	    const top = ev.pageY + yOffset;

		cat.style.left = `${left}px`
		cat.style.top = `${top}px`
	})
</script>

<main>
	<h1>Play with the goodboy 🐱</h1>
	<img id="goodboy" src="./favicon.png" alt="goodboy">
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #dd8cb2;
		text-transform: uppercase;
		font-size: 3em;
		font-weight: 400;
	}

	#goodboy{
		width: 100px;
		border: 5px solid #d4abab;
		border-radius: 5px;
		position: absolute;
		transform:translate(-50%,20%);
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>