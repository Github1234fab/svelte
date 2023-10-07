<script>
	export let text;
	export let src;
	export let paragraph;
</script>

<div class="card-body">
	<img class="img-cards" src={src} alt="">
	<h5 class="card-title">{text}</h5>
	<p class="card-text">{paragraph}</p>
	<a href="e" class="btn btn-primary">En savoir plus ...</a>
</div>

<style>
	.card-body {
		background-image: repeating-linear-gradient(
				135deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				45deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				67.5deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				135deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				45deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				112.5deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				112.5deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				45deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				22.5deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				45deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				22.5deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				135deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				157.5deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				67.5deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			repeating-linear-gradient(
				67.5deg,
				hsla(264, 0%, 88%, 0.03) 0px,
				hsla(264, 0%, 88%, 0.03) 1px,
				transparent 1px,
				transparent 12px
			),
			linear-gradient(90deg, rgb(151, 26, 210), rgb(57, 199, 205));
		display: flex;
		/* flex-direction: column; */
		justify-content: center;
		align-items: center;
		gap: 20px;
		width: 40%;
		height: 400px;
		background-color: rgba(255, 255, 255, 0.909);
		backdrop-filter: blur(10px);
		border-radius: 10px;
	}

	.img-cards {
		height: 200px;
		width: 100%;
		box-shadow: inset 1px 1px 6px var(--colorB);
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
