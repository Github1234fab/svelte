<script>
	export let text;
	export let paragraph;
	// export let cardNumber;
	export let backgroundImage;
	import BtnSlideLeft from './Btn-slide-left.svelte';

	let btnText = [
		{
			key: 1,
			name: 'Constituer mon dossier de pré-admission'
		},
		{
			key: 2,
			name: "Prendre mon rendez-vous d'anesthésie",
		},
		{
			key: 3,
			name: 'Préparation préopératoires'
		}
	];
</script>

<div class="card-body card" style="background-image: url({backgroundImage});">
	<!-- <div class="card-number">{cardNumber}</div> -->
	<div class="wrapper-text-cards">
		<h5 class="card-title">{text}</h5>
		<p class="card-text">{paragraph}</p>
		{#each btnText as name (name.key)}
			<BtnSlideLeft btnSlideName={name.name} />
		{/each}
	</div>
</div>

<style>
	.card-body {
		margin-top: 50px;
		position: relative;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		align-content: center;
		padding: 60px;
		gap: 30px;
		width: 40%;
		height: fit-content;
		box-shadow: 1px 1px 5px var(--colorB);
		background-color: rgba(255, 255, 255, 0.909);
		border-radius: 10px;
		background-size: 130%;
		background-position: center;
		background-repeat: no-repeat;
	}
	/* .card-number {
		position: absolute;
		width: 100px;
		height: 100px;
		border-radius: 50%;
		background-color: rgba(0, 0, 255, 0.179);
		-webkit-backdrop-filter: blur(20px);
		backdrop-filter: blur(20px);
		top: -60px;
		left: -70px;
		color: white;
		font-size: 2em;
		font-weight: bolder;
		display: flex;
		align-items: center;
		justify-content: center;
	} */

	.card-title {
		font-size: 1.5em;
		text-transform: uppercase;
		text-align: center;
	}

	.card-text {
		font-size: 1em;
		width: 100%;
		text-align: center;
	}

	/* .card:nth-child(odd) {
		margin-left: 300px; 
	}
	.card:nth-child(even) {
		margin-left: -300px; 
	} */

	.wrapper-text-cards {
		background-color: rgba(255, 255, 255, 0.293);
		backdrop-filter: blur(10px);
		padding: 30px;
		display: flex;
		flex-direction: column;
		gap: 30px;
		justify-content: center;
	}
</style>
