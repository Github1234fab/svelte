<script>
	export let text;
	export let src;
	export let paragraph;
	export let textButton;
</script>

<div class="card-body">
	<img class="img-cards" {src} alt="" />
	<h5 class="card-title">{text}</h5>
	<p class="card-text">{paragraph}</p>
	<a href="e" class="btn btn-primary">En savoir plus ...</a>
</div>

<style>
	.card-body {
		display: flex;
                flex-direction: column;
		justify-content: center;
		align-items: center;
                gap: 20px;
		width: 40%;
		height: 400px;
		background-color: rgba(255, 255, 255, 0.395);
                backdrop-filter: blur(10px);
	}

	.img-cards {
		height: 200px;
		width: auto;
		box-shadow: 1px 1px 6px var(--colorB);
	}

	.card-text {
		font-size: 1em;
	}
	.btn {
		width: 5em;
		height: 3em;
                text-decoration: none;
                background-color: var(--colorA);
                color: white;
                border: none;
                box-shadow: 1px 1px 6px (var(--colorB));
                border-radius: 5px;
	}
</style>
