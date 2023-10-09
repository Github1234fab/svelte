<script>
	export let btnSlideName;
</script>

<a href="e" class="btn"><span class="btn-txt"> {btnSlideName}</span> </a>

<style>
	.btn {
		position: relative;
		padding: 20px;
		text-decoration: none;
		background-color: var(--colorA);
		color: white;
		border: none;
		box-shadow: 1px 1px 6px var(--colorB);
		border-radius: 5px;
		overflow: hidden;
		z-index: 1;
	}

	.btn::after {
		content: '';
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		background-color: var(--colorB);
		transform: translateX(-100%); /* Initialement, déplacez-le complètement à gauche */
		transition: transform 0.7s ease-in-out;
		z-index: -1;
	}
	.btn:hover::after {
		transform: translateX(0); /* Au survol, déplacez-le à sa position initiale */
	}
	.btn-txt {
		z-index: 1;
	}
</style>
