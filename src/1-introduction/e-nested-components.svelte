<script>
  import Styling from "./d-styling.svelte";
</script>

<div id="nested-componets">
  <h2>This component imports the component below</h2>
  <Styling />
</div>

<style>
  h2 {
    color: green;
  }
</style>
