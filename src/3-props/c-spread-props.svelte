<script>
  import NestedComponent from "./nested-component.svelte";

  const data = {
    header: "This is a spreaded header",
    text: "This is a spreaded paragraph",
  };
</script>

<div id="spread-props">
  <NestedComponent {...data} />
  <hr />
</div>
