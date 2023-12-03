<script lang="ts">
    let counter: number;
    $: counter = 0;
    const increment = () => (counter += 1);
    const decrement = () => (counter -= 1);
</script>

<h1>Basic counter example</h1>
<button on:click={increment}> Increment </button>
<button on:click={decrement}> Decrement </button>
<p>
    Counter value is {counter}
</p>
