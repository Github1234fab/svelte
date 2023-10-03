<script>
	import ButtonCircle from './ButtonCircle.svelte';

	let buttonData = [
		{ text: 'Consultation' },
		{ text: 'Ambulatoire' },
		{ text: 'Séjours' },
		{ text: 'Chirurgie' }
	];
</script>

<div class="wrapper-buttonsCircle">
                {#each buttonData as buttonItem (buttonItem.text)}
	<ButtonCircle text={buttonItem.text} />
{/each}
</div>

<style>
        .wrapper-buttonsCircle {
                display: flex;
                flex-wrap: wrap;
                justify-content: space-around;
                align-items: center;
                margin-top: -50px;
        }
</style>
