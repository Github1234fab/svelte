<script></script>

<div class="wrapper-images-sectionB">
	<div class="wrapper-img"><div class="img1 image" /></div>
	<div class="wrapper-img"><div class="img2 image" /></div>
	<div class="wrapper-img"><div class="img3 image" /></div>
	<div class="wrapper-img"><div class="img4 image" /></div>
</div>

<style>
	.wrapper-images-sectionB {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-around;
		align-items: center;
		width: 100vw;
		height: 400px;
		padding: 10px;
		margin-top: 200px;
		cursor: pointer;
	}
	.wrapper-img{
		width: 400px;
		height: 100%;
		overflow: hidden;
			box-shadow: 0px 1px 4px var(--colorB);
	}
	.image {
		background-repeat: no-repeat;
		background-size: cover;
		background-position: center;
		width: 100%;
		height: 100%;
	
		border: none;
		opacity: 0.9;
		transition: 0.7s ease-in-out;
	}
	.image:hover {
		opacity: 1;
	transform: scale(1.2);
	}

	.img1 {
		background-image: url('https://images.unsplash.com/photo-1551601651-09492b5468b6?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=3013&q=80');
	}
	.img2 {
		background-image: url('https://images.unsplash.com/photo-1621021544363-02108c715c1b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2936&q=80');
	}
	.img3 {
		background-image: url('https://images.unsplash.com/photo-1551190822-a9333d879b1f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2940&q=80');
	}

	.img4 {
		background-image: url('https://images.unsplash.com/photo-1551601651-bc60f254d532?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTF8fGNoaXJ1cmdpZSUyMHJlY29uc3RydWN0cmljZXxlbnwwfHwwfHx8MA%3D%3D&auto=format&fit=crop&w=800&q=60');
	}
</style>
