<script>
	let input = '';
	console.log(input);
	//         function collectName (e){
	// let inputName = e.target.value;
	//    console.log(inputName);
	//         }
</script>

<input class="input" type="text" bind:value={input} placeholder="login"/>
<p>{input}</p>

<style>
	.input {
		width: 40%;
		height: 3em;
                font-size: 1em;
		box-shadow: inset 1px 0px 6px black;
                text-align: center;
                padding: 20px;
	}
</style>
