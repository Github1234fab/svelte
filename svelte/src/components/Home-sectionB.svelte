<script>
	import ImagesSectionB from './Images-sectionB.svelte';
</script>

<section class="B-section">
	<h2 class="section-B-title">
		Notre équipe médicale est composée de chirurgiens de grande renommée mondiale.
	</h2>
	<p class="section-B-docteurs">
		Dr. Jean-Louis Garient, Dr. Dominique Fiedierck, Dr. Alain Badout, Dr.  Monique Verot, Dr.Hugo
		Bouvier, Dr. Capucine Monart, Dr. Stephen Groden, Dr. Alan Smith Jr, Dr. Afna Azrdaff, Dr. Amid
		Maalouf, Dr. Lorenzo Marenzi, Dr. Lawrence Jacob ...
	</p>
	<ImagesSectionB />
</section>

<style>
	.B-section {
		width: 100vw;
		height: 1000px;
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
		background-position: 100%;
		margin-top: -100px;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.section-B-title {
		font-size: 2.4em;
		color: rgb(14, 13, 13);
		font-weight: 200;
		margin-top: 140px;
	}
	.section-B-docteurs {
		margin-top: 50px;
		text-align: left;
		font-weight: 200;
		width: 70%;
	}
</style>
