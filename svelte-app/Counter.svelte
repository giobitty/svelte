<!-- Counter.svelte -->

<script>
    let count = 0;
  
    function increment() {
      count += 1;
    }
  
    function decrement() {
      count -= 1;
    }
  </script>
  
  <main>
    <h1>Counter App</h1>
    <p>Count: {count}</p>
    <button on:click={increment}>Increment</button>
    <button on:click={decrement}>Decrement</button>
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
      font-size: 2em;
    }
  
    p {
      font-size: 1.5em;
      margin: 1em 0;
    }
  
    button {
      font-size: 1em;
      padding: 0.5em 1em;
      margin: 0.5em;
    }
  </style>
  