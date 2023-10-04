<script>
	import CardsHomeSectionC from './Cards-HomeSectionC.svelte';

	let cardsText = [
		{
			text: 'aerjbfakeljrbvlejarbv',
			paragraph: 'kdsjbfksjdbf',
			textButton: 'vhksfbkvhsbfkv',
			src: 'https://www.montpellier-chirurgie-plastique-esthetique.com/assets/img/page/17/large/fr/entree-clinique-saint-jean-montpellier.jpg'
		},
		{
			text: 'aerjbfakeljrbvlejarbv',
			paragraph: 'kdsjbfksjdbf',
			textButton: 'vhksfbkvhsbfkv',
			src: 'https://www.montpellier-chirurgie-plastique-esthetique.com/assets/img/page/17/large/fr/entree-clinique-saint-jean-montpellier.jpg'
		},
		{
			text: 'aerjbfakeljrbvlejarbv',
			paragraph: 'kdsjbfksjdbf',
			textButton: 'vhksfbkvhsbfkv',
			src: 'https://www.montpellier-chirurgie-plastique-esthetique.com/assets/img/page/17/large/fr/entree-clinique-saint-jean-montpellier.jpg'
		}
	];
</script>

<section class="section-C">
	{#each cardsText as card (card.text)}
		<CardsHomeSectionC
			text={card.text}
			src={card.src}
			textButton={card.textButton}
			paragraph={card.paragraph}
		/>
	{/each}
</section>

<style>
	.section-C {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		gap: 10px;
		width: 100vw;
		height: 1000px;
		background-image: radial-gradient(
				circle at 85% 1%,
				hsla(190, 0%, 93%, 0.05) 0%,
				hsla(190, 0%, 93%, 0.05) 96%,
				transparent 96%,
				transparent 100%
			),
			radial-gradient(
				circle at 14% 15%,
				hsla(190, 0%, 93%, 0.05) 0%,
				hsla(190, 0%, 93%, 0.05) 1%,
				transparent 1%,
				transparent 100%
			),
			radial-gradient(
				circle at 60% 90%,
				hsla(190, 0%, 93%, 0.05) 0%,
				hsla(190, 0%, 93%, 0.05) 20%,
				transparent 20%,
				transparent 100%
			),
			radial-gradient(
				circle at 79% 7%,
				hsla(190, 0%, 93%, 0.05) 0%,
				hsla(190, 0%, 93%, 0.05) 78%,
				transparent 78%,
				transparent 100%
			),
			radial-gradient(
				circle at 55% 65%,
				hsla(190, 0%, 93%, 0.05) 0%,
				hsla(190, 0%, 93%, 0.05) 52%,
				transparent 52%,
				transparent 100%
			),
			linear-gradient(440deg, rgb(37, 56, 222), rgb(96, 189, 244));
	}
</style>
