<script>
	export let name;

	let num1 = 0 ;
	let num2 = 0 ;
	let sum = 0 ;
	function result () {
		num1 = Math.floor((Math.random()*100) +1);
		num2 = Math.floor((Math.random()*100) +1);

	}	
	function initsum () {
			 sum = num1 + num2;
	}



</script>

<main>
	<h1>Hello {name}!</h1>
	<p>
		Two Random numbers {num1} and {num2}
	</p>
	<button on:click= {initsum}>
	{sum}
	</button>
	<p>
		sum of {num1} + {num2} = {sum}
	</p>
	<button on:click={result}> Refresh </button>
	
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