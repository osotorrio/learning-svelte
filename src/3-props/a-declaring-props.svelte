<script>
  import NestedComponent from "./nested-component.svelte";

  const messageToChild = "How are you?";
</script>

<NestedComponent message={messageToChild} />
<hr />
