<script>
  let toggle = false;

  function toggleState() {
    toggle = !toggle;
  }
</script>

<button on:click={toggleState}>Toggle</button>

{#if toggle}
  <h2>Display if true</h2>
{/if}

{#if !toggle}
  <p>Display if false</p>
{/if}
<hr />

<style>
  h2 {
    color: lightblue;
  }

  p {
    color: red;
  }
</style>
