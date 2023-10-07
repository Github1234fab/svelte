<script>
	let prevScrollY = 0;
	let headerElement;

	function displayHeader() {
		window.addEventListener('scroll', () => {
			const currentScrollY = window.scrollY;

			if (currentScrollY > prevScrollY) {
				// Défilement vers le bas
				headerElement.style.opacity = 0;
				headerElement.style.transition = 'opacity 0.9s ease-in-out';
			} else {
				// Défilement vers le haut
				headerElement.style.opacity = 1;
				// headerElement.style.transition = 'opacity 0.7s ease-in-out';
			}

			prevScrollY = currentScrollY;
		});
	}
</script>

<header bind:this={headerElement} class="header" use:displayHeader>
	<div class="wrapper-logo">
		<div class="logo" />
		<h1>Elinxia</h1>
	</div>
	<ul>
		<a href=">">Chirurgie des seins</a>
		<a href=">">Chirurgie du corps</a>
		<a href=">">Chirurgie du visage</a>
		<a href=">">Chirurgie capillaire</a>
		<a href=">">Médecine esthétique</a>
	</ul>
</header>

<style>
	header {
		width: 100%;
		display: flex;
		justify-content: space-around;
		align-items: center;
		padding: 20px;
		height: 80px;
		position: fixed;
		background-color: white;
		z-index: 999999;
	}
	.wrapper-logo {
		display: flex;
		gap: 10px;
	}

	.logo {
		width: 3em;
		height: 3em;
		background-image: url('../assets/LogoHeader.png');
		background-position: center;
		background-size: cover;
	}

	ul {
		display: flex;
		justify-content: space-around;
		width: 90%;
	}
	a {
		text-decoration: none;
		color: black;
		font-weight: 900;
	}
	a:hover {
		text-decoration: underline;
		font-weight: 900;
	}
</style>
