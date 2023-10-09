<script>
	import CardsHomeSectionC from './Cards-HomeSectionC.svelte';
	import stetoscopeImage from '../assets/Stetoscope.png';
	import medicalicon from '../assets/medicalicons.png';
	import preopImage from '../assets/preoperatoire.png';

	let cardsText = [
		{
			key: 1,

			text: 'ADMISSION DU PATIENT',
			paragraph:
				'Pour que votre admission à la clinique Elinxia puisse être prise en compte, veuillez passer par les 3 étapes suivantes SVP!'
			// Number: '1'
		}
		// {
		// 	key: 2,
		// 	backgroundImage: stetoscopeImage,
		// 	text: "Consultation d'anesthésie",
		// 	paragraph:
		// 		"Le secrétariat vous a communiqué votre date d'intervention. Maintenant prenez rendez-vous avec votre anesthésite.",
		// 	Number: '2'
		// },
		// {
		// 	key: 3,
		// 	backgroundImage: preopImage,
		// 	text: 'Préparation préopératoire',
		// 	paragraph:
		// 		" Obtenez l'heure de votre convocation, ainsi que toutes les directives relatives à votre intervention.",
		// 	Number: '3'
		// }
	];
</script>

<section class="section-C">
	<!-- <h3>Parcours du patient</h3> -->
	{#each cardsText as card (card.key)}
		<CardsHomeSectionC src={card.src} text={card.text} paragraph={card.paragraph} />
	{/each}
</section>

<style>
	.section-C {
		display: flex;
		width: 100vw;
		height: 1000px;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		padding: 20px;
		gap: 10px;
		margin-top: -100px;
		background-image: linear-gradient(
				0,
				hsla(80, 87%, 72%, 0.44) 0%,
				hsla(80, 87%, 72%, 0.44) 12.5%,
				hsla(125, 87%, 72%, 0.44) 12.5%,
				hsla(125, 87%, 72%, 0.44) 25%,
				hsla(170, 87%, 72%, 0.44) 25%,
				hsla(170, 87%, 72%, 0.44) 37.5%,
				hsla(215, 87%, 72%, 0.44) 37.5%,
				hsla(215, 87%, 72%, 0.44) 50%,
				hsla(260, 87%, 72%, 0.44) 50%,
				hsla(260, 87%, 72%, 0.44) 62.5%,
				hsla(305, 87%, 72%, 0.44) 62.5%,
				hsla(305, 87%, 72%, 0.44) 75%,
				hsla(350, 87%, 72%, 0.44) 75%,
				hsla(350, 87%, 72%, 0.44) 87.5%,
				hsla(35, 87%, 72%, 0.44) 87.5%,
				hsla(35, 87%, 72%, 0.44) 100%
			),
			linear-gradient(
				90deg,
				hsl(348, 83%, 76%) 0%,
				hsl(348, 83%, 76%) 12.5%,
				hsl(33, 83%, 76%) 12.5%,
				hsl(33, 83%, 76%) 25%,
				hsl(78, 83%, 76%) 25%,
				hsl(78, 83%, 76%) 37.5%,
				hsl(123, 83%, 76%) 37.5%,
				hsl(123, 83%, 76%) 50%,
				hsl(168, 83%, 76%) 50%,
				hsl(168, 83%, 76%) 62.5%,
				hsl(213, 83%, 76%) 62.5%,
				hsl(213, 83%, 76%) 75%,
				hsl(258, 83%, 76%) 75%,
				hsl(258, 83%, 76%) 87.5%,
				hsl(303, 83%, 76%) 87.5%,
				hsl(303, 83%, 76%) 100%
			);
	}
	/* .section-C h3 {
		font-size: 3em;
		color: var(--colorB);
		font-weight: 900;
		padding: 20px;
		text-transform: uppercase;
		margin-top: 100px;
	} */
</style>
