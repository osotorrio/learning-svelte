<script>
  let count = 0;

  function incrementCount() {
    count += 1;
  }

  $: if (count > 10) {
    console.error(`Count is very high: ${count}`);
  }
</script>

<div id="statements">
  <button on:click={incrementCount}>Clicked {count}</button>
  <hr />
</div>
