<script>
	export let name;
	let color = 'black';

	const handleClick = () => {
		color = 'blue';
	};

</script>

<main>
	<h1>Hello {name}!</h1>
	<h3>hi, my name is one!</h3>
	<p style='color: {color}'>{color} beammmmmmm!!!!!</p>
	<button on:click={handleClick}>update jean color</button>
	<input type='text' bind:value={color} />

</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>