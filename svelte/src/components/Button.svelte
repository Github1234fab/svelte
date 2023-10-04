<script>
</script>

<div class="wrapper-button">
	<svg
		class="button"
		width="245"
		height="102"
		viewBox="0 0 245 102"
		fill="grey"
		xmlns="http://www.w3.org/2000/svg"
	>
		<rect class="rect" width="245" height="102" fill="#0779bf" />
	</svg>
	<h3 class="button-text">Découvrir</h3>
</div>

<style>
	.wrapper-button {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: space-around;
		height: 170px;
	}
	.button {
		border-radius: 5px;
		position: relative;
		cursor: pointer;
	}
	.rect {
		stroke-dasharray: 1000;
		stroke-dashoffset: 1000;
		stroke: var(--colorC);
		stroke-width: 1px;
	}
	@keyframes dash {
		to {
			stroke-dashoffset: 0;
		}
	}
	.button:hover .rect {
		stroke-width: 5px;
		animation: dash 1.8s linear forwards;
		filter: drop-shadow(2px 2px 100px #d7e0e6);
	}
	.button:hover {
		transform: scale(1.05);
		transition: 0.3s ease-in-out;
		filter: drop-shadow(0px 0px 100px #a8cbe1);
	}
	.button-text {
		font-size: 1.4em;
		font-weight: 600;
		color: white;
		margin-top: -170px;
		z-index: 1;
		pointer-events: none;
	}
	
</style>
