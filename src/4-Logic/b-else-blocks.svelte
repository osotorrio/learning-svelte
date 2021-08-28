<script>
  let toggle = false;

  function toggleState() {
    toggle = !toggle;
  }
</script>

<div id="else-blocks">
  <button on:click={toggleState}>Toggle</button>

  {#if toggle}
    <h2>Display if true</h2>
  {:else}
    <p>Display if false</p>
  {/if}
  <hr />
</div>

<style>
  h2 {
    color: lightblue;
  }

  p {
    color: red;
  }
</style>
