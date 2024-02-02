<!-- NumberGenerator.svelte -->

<script>
    let numbers = [];
  
    function generateNumbers() {
      numbers = Array.from({ length: 5 }, () => Math.floor(Math.random() * 100));
    }
  
    function sortNumbers() {
      numbers = numbers.slice().sort((a, b) => a - b);
    }
  </script>
  
  <main>
    <h2>Number Generator</h2>
    <button on:click={generateNumbers}>Generate Numbers</button>
    <p>Numbers: {numbers.join(', ')}</p>
    <button on:click={sortNumbers}>Sort Numbers</button>
  </main>
  
  <!--creiamo style diversi per questo component-->
  <style>
    main {
      text-align: center;
      padding: 1em;
      max-width: 240px;
      margin: 0 auto;
      background-color: #e0e0e0;
    }
  
    h2 {
      color: #0070f3;
      font-size: 1.5em;
    }
  
    p {
      font-size: 1em;
      margin: 1em 0;
    }
  
    button {
      font-size: 1em;
      padding: 0.5em 1em;
      margin: 0.5em;
    }
  </style>
  