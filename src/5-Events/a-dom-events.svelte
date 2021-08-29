<script>
  let value = 0;
  function moveButton(event) {
    value += 20;
    event.target.style.bottom = `${value}px`;
  }
</script>

<div id="dom-events">
  <h2 on:focus={moveButton} on:mouseover={moveButton}>
    Pass mouse over to move this
  </h2>
  <hr />
</div>

<style>
  h2 {
    position: relative;
    border: 5px solid red;
  }
</style>
