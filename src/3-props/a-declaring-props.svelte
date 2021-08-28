<script>
  import NestedComponent from "./nested-component.svelte";

  const header = "This is a header";
  const text = "This is paragraph";
</script>

<NestedComponent {header} {text} />
<hr />
