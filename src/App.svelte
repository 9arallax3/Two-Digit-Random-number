<script>
  let result = 0;
  let num1 = 0;
  let num2 = 0;
  let sum1,
    sum2,
    sum3,
    sum4,
    sum5 = 0;
  function RandomNumberGenerator() {
    num1 = Math.floor(Math.random() * 100 + 1);
    num2 = Math.floor(Math.random() * 100 + 1);
  }

  function add() {
    result = num1 + num2;
  }

  function sub() {
    result = num1 - num2;
  }

  function multi() {
    result = num1 * num2;
  }
  function modulus() {
    result = num1 % num2;
  }
  function division() {
    result = num1 / num2;
  }
</script>

<main>
  <h1>Math For Class - 1</h1>
  <br />
  <br />
  <br />

  <h2>
    Two Random numbers {num1} and {num2} <br />

    <br />
  </h2>

  <h2>
    {result}
  </h2>

  <br />
  <br />

  <p>
    <button on:click={add}>Add </button>
    <button on:click={sub}>Sub</button>
    <button on:click={multi}>Multiplication</button>
    <button on:click={modulus}>Modulus</button>
    <button on:click={division}>Division</button>
  </p>

  <button on:click={RandomNumberGenerator}> Refresh </button>
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }
  h2 {
	
    color: aqua;
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
