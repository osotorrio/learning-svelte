<script>
  let count = 0;

  function incrementCount() {
    count += 1;
  }
</script>

<button on:click={incrementCount}>
  You clicked this {count}
  {count === 1 ? "time" : "times  "}
</button>
<hr />
