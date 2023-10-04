<script>
	import Button from '../components/Button.svelte';
	import ButtonCircle from './ButtonCircle.svelte';

	let buttonData = [
		{ text: 'Consultation', icon: "fa-calendar-check" },
		{ text: 'Secrétariat', icon: "fa-envelope" },
		{ text: 'Séjours', icon: "fa-bed" },
		{ text: 'Chirurgie', icon: "fa-laptop-medical" }
	];
</script>

<body>
	<section class="A-section">
		<div class="image-visage" />
		<div class="wrapper-sectionA-title">
			<h1 class="bouton">Elinxia, Clinique de chirurgie reconstructrice, plastique et esthétique</h1>
			<Button />
		</div>
		
	</section>
	<div class="wrapper-buttonsCircle">
		{#each buttonData as buttonItem (buttonItem.text)}
			<ButtonCircle text={buttonItem.text} icon={buttonItem.icon}/>
		{/each}
	</div>
	
</body>

<style>
	body {
		background-color: white;
		font-family: poppins;
	}
	.A-section {
		display: grid;
		align-items: center;
		align-content: center;
		grid-template-columns: 1fr 1fr;
		width: 100vw;
		height: 600px;
		overflow: hidden;
		background-image: radial-gradient(
				circle at 67% 83%,
				hsla(317, 0%, 96%, 0.05) 0%,
				hsla(317, 0%, 96%, 0.05) 1%,
				transparent 1%,
				transparent 5%,
				transparent 5%,
				transparent 100%
			),
			radial-gradient(
				circle at 24% 80%,
				hsla(317, 0%, 96%, 0.05) 0%,
				hsla(317, 0%, 96%, 0.05) 27%,
				transparent 27%,
				transparent 63%,
				transparent 63%,
				transparent 100%
			),
			radial-gradient(
				circle at 23% 5%,
				hsla(317, 0%, 96%, 0.05) 0%,
				hsla(317, 0%, 96%, 0.05) 26%,
				transparent 26%,
				transparent 82%,
				transparent 82%,
				transparent 100%
			),
			radial-gradient(
				circle at 21% 11%,
				hsla(317, 0%, 96%, 0.05) 0%,
				hsla(317, 0%, 96%, 0.05) 35%,
				transparent 35%,
				transparent 45%,
				transparent 45%,
				transparent 100%
			),
			radial-gradient(
				circle at 10% 11%,
				hsla(317, 0%, 96%, 0.05) 0%,
				hsla(317, 0%, 96%, 0.05) 21%,
				transparent 21%,
				transparent 81%,
				transparent 81%,
				transparent 100%
			),
			radial-gradient(
				circle at 19% 61%,
				hsla(317, 0%, 96%, 0.05) 0%,
				hsla(317, 0%, 96%, 0.05) 20%,
				transparent 20%,
				transparent 61%,
				transparent 61%,
				transparent 100%
			),
			radial-gradient(
				circle at 13% 77%,
				hsla(317, 0%, 96%, 0.05) 0%,
				hsla(317, 0%, 96%, 0.05) 63%,
				transparent 63%,
				transparent 72%,
				transparent 72%,
				transparent 100%
			),
			radial-gradient(
				circle at 30% 93%,
				hsla(317, 0%, 96%, 0.05) 0%,
				hsla(317, 0%, 96%, 0.05) 33%,
				transparent 33%,
				transparent 82%,
				transparent 82%,
				transparent 100%
			),
			linear-gradient(281deg, rgb(22, 176, 207), rgb(103, 7, 215));
	}
	.A-section h1 {
		color: white;
		font-size: 2.4em;
		width: 100%;
		margin: auto;
		font-weight: bolder;
	}
	.image-visage {
		grid-column: 1/2;
		height: 830px;
		width: 100%;
		margin-top: 100px;
		background-image: url('../assets/visage-Asection.png');
		background-size: contain;
		background-position: center;
		background-repeat: no-repeat;
	}
	.wrapper-sectionA-title {
		grid-column: 2/3;
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		gap: 20px;
	}
	.wrapper-buttonsCircle {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-around;
		align-items: center;
		margin-top: -50px;
		
	}
</style>
