<script>
  import NestedComponent from "./nested-component.svelte";

  const data = {
    header: "This is a header",
    text: "This is a paragraph",
  };
</script>

<NestedComponent props={data} />
<hr />
