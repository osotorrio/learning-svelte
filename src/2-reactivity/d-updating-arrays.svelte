<script>
  let numbers = [];

  function addNumberToArray() {
    numbers = [...numbers, numbers.length + 1];
  }
</script>

<div id="updating-arrays">
  <button on:click={addNumberToArray}>Add number: {numbers.length + 1}</button>
  <p>Numbers: {numbers.join(", ")}</p>
  <hr />
</div>
