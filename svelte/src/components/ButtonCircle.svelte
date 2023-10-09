<script>
	export let text;
	export let icon;
</script>

<button class="button-circle">
	<span class="icon">
		<i class="fa {icon}" />
	</span>
	<span class="text">{text}</span>
</button>

<style>
	.button-circle {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		gap: 13px;
		width: 150px;
		height: 150px;
		border-radius: 50%;
		background-color: var(--colorA);
		color: white;
		border: solid white 4px;
		font-weight: 500;
		font-size: 1.1em;
		z-index: 9999;
		transition: 0.2s ease-in-out;
	}
	.button-circle:hover {
		
                /* box-shadow: 0px 0px 50px  white; */
		transform: scale(1.1);
         
	}
	.icon {
		font-size: 2em;
	}
      
</style>
