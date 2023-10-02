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
	<rect class="rect" width="245" height="102" fill="#0779bf" stroke="#96EC85" />
</svg>
<h3 class="button-text">Découvrir</h3>
</div>

<style>
      .wrapper-button{
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: space-around;
            height: 170px;
          
      }
	.button {
		filter: drop-shadow(5px 5px 5px #044268);
		border-radius: 5px;
            position: relative;
            cursor: pointer
		
	}
	.rect {
		stroke-dasharray: 1000;
		stroke-dashoffset: 1000;
            
	}
	@keyframes dash {
		to {
			stroke-dashoffset: 0;
		}
	}
	.button:hover .rect {
		stroke-width: 4px;
		animation: dash 1.5s linear forwards;
	}
      .wrapper-button:hover .button{
          filter: drop-shadow(0px 0px 100px #d7e0e6);
            transform: scale(1.05);
            transition: 0.5s ease-in-out;
      }
	.button-text {
		font-size: 1.4em;
		font-weight: 600;
		color: white;
            margin-top: -170px;
            z-index: 99;
	}
</style>
