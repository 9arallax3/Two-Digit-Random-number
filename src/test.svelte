<script>
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
