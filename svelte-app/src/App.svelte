<!-- App.svelte -->

<script>
	import Counter from '../Counter.svelte';
	//importo l altro componente per vederlo sotto al primo
	import NumberGenerator from '../NumberGenerator.svelte';
  </script>
  
  <main>
	<Counter />
	<NumberGenerator />
  </main>
  
  <style>
	main {
	  text-align: center;
	  padding: 1em;
	  max-width: 240px;
	  margin: 0 auto;
	}
  </style>
  