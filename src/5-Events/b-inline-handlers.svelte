<script>
  let position = { x: 0, y: 0 };
</script>

<div id="inline-handlers">
  <div on:mousemove={(e) => (position = { x: e.clientX, y: e.clientY })}>
    The mouse position is {position.x} x {position.y}
  </div>
  <hr />
</div>

<style>
  div {
    width: 100%;
    height: 100%;
  }
</style>
