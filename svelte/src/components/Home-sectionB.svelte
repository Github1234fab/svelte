<script>
	import ImagesSectionB from './Images-sectionB.svelte';
</script>

<section class="B-section">
	<h2 class="section-B-title">
		Une équipe d'experts internationaux en chirurgie plastique et reconstructrice.
	</h2>
	<div class="wrapper-doctorsName">
		<ul class="doctors-name">
			<li>Dr. Dominique Fiedelick</li>
			<li>Dr. Alain Badout</li>
			<li>Dr. Monique Verot</li>
			<li>Dr. Lorenzo Marenzi</li>
			<li>Dr. Amid Maalouf</li>
		</ul>
		<ul class="doctors-name">
			<li>Dr.Hugo Bouvier</li>
			<li>Dr. Capucine Monart</li>
			<li>Dr. Stephen Groden</li>
			<li>Dr. Lorenzo Marenzi</li>
			<li>Dr. Alan Smith</li>
		</ul>
		<ul class="doctors-name">
			<li>Dc. Marcus Cortesi</li>
			<li>Dr. Dina Wahington</li>
			<li>Dr. Ali Boudamief</li>
			<li>Dr. Shera Hoshen</li>
			<li>Dr. Eliot Murphy</li>
		</ul>
	</div>

	<ImagesSectionB />
</section>

<style>
	.B-section {
		width: 100%;
		height: fit-content;
		margin-top: -100px;
		margin-bottom: 20px;
		display: flex;
		flex-direction: column;
		align-items: content;
		justify-content: center;
		align-items: center;
		background-position: 100%;
		background-size: cover;
		background-color: rgb(193, 231, 68);
		background-image: radial-gradient(
				circle at 13% 47%,
				rgba(140, 140, 140, 0.03) 0%,
				rgba(140, 140, 140, 0.03) 25%,
				transparent 25%,
				transparent 100%
			),
			radial-gradient(
				circle at 28% 63%,
				rgba(143, 143, 143, 0.03) 0%,
				rgba(143, 143, 143, 0.03) 16%,
				transparent 16%,
				transparent 100%
			),
			radial-gradient(
				circle at 81% 56%,
				rgba(65, 65, 65, 0.03) 0%,
				rgba(65, 65, 65, 0.03) 12%,
				transparent 12%,
				transparent 100%
			),
			radial-gradient(
				circle at 26% 48%,
				rgba(60, 60, 60, 0.03) 0%,
				rgba(60, 60, 60, 0.03) 6%,
				transparent 6%,
				transparent 100%
			),
			radial-gradient(
				circle at 97% 17%,
				rgba(150, 150, 150, 0.03) 0%,
				rgba(150, 150, 150, 0.03) 56%,
				transparent 56%,
				transparent 100%
			),
			radial-gradient(
				circle at 50% 100%,
				rgba(25, 25, 25, 0.03) 0%,
				rgba(25, 25, 25, 0.03) 36%,
				transparent 36%,
				transparent 100%
			),
			radial-gradient(
				circle at 55% 52%,
				rgba(69, 69, 69, 0.03) 0%,
				rgba(69, 69, 69, 0.03) 6%,
				transparent 6%,
				transparent 100%
			),
			linear-gradient(90deg, rgb(255, 255, 255), rgb(255, 255, 255));
	}

	.section-B-title {
		font-size: 2.4em;
		color: rgb(14, 13, 13);
		font-weight: 200;
		text-align: center;
		margin-top: 200px;
	}
	.wrapper-doctorsName {
		display: flex;
		justify-content: space-around;
		width: 70%;
		margin-top: 100px;
	}
	.doctors-name li {
		list-style-type: none;
		font-family: Cambria;
		padding: 10px;
		font-size: 1.3em;
	}
</style>
