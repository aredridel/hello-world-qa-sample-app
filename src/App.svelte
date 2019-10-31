<script>
	let name = 'world';
	let color = "black";
</script>

<h1>Hello <span style="color: {color}">{name}</span>!</h1>

<button on:click={() => { color = "red" }}>
	 Go!
</button>

<button on:click={() => { color = "black" }} >
	Stop
</button>

<form on:submit|preventDefault>
	
	<fieldset>
		<legend>
			Fields
		</legend>
		<label>Name <input bind:value={name} type="text"></label>
	</fieldset>
</form>