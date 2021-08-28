<script>
  let count = 0;
  $: doubled = count * 2;

  function incrementCount() {
    count += 1;
  }
</script>

<button on:click={incrementCount}>
  You clicked {count} times which its double is equal to {doubled}
</button>
<hr />
