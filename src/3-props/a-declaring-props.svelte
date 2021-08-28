<script>
  import NestedComponent from "./nested-component.svelte";

  const header = "This is a header";
  const text = "This is paragraph";
</script>

<div id="declaring-props">
  <NestedComponent {header} {text} />
  <hr />
</div>
