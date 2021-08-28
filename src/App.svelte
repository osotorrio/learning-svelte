<script>
  export let name;
  import Basics from "./1-introduction/a-basics.svelte";
  import AddingData from "./1-introduction/b-adding-data.svelte";
  import DynamicAttributes from "./1-introduction/c-dynamic-attributes.svelte";
  import Styling from "./1-introduction/d-styling.svelte";
  import Nested from "./1-introduction/e-nested-components.svelte";
  import HtmlTag from "./1-introduction/f-html-tags.svelte";
  import Assignments from "./2-reactivity/a-assignments.svelte";
  import Declarations from "./2-reactivity/b-declarations.svelte";
  import Statements from "./2-reactivity/c-statements.svelte";
  import UpdateArray from "./2-reactivity/d-updating-arrays.svelte";
  import UpdateObject from "./2-reactivity/d-updating-objects.svelte";
  import DeclaringProps from "./3-props/a-declaring-props.svelte";
  import DefaultProps from "./3-props/b-default-props.svelte";
  import SpreadProps from "./3-props/c-spread-props.svelte";
  import IfBlocks from "./4-Logic/a-if-blocks.svelte";
  import ElseBlocks from "./4-Logic/b-else-blocks.svelte";
  import ElseIfBlocks from "./4-Logic/c-else-if-blocks.svelte";
  import EachBlock from "./4-Logic/d-each-blocks.svelte";
  import KeyedEachBlock from "./4-Logic/e-keyed-each-blocks.svelte";
</script>

<main>
  <h1>Hello {name}!</h1>
  <p>
    Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
    how to build Svelte apps.
  </p>
  <Basics />
  <AddingData />
  <DynamicAttributes />
  <Styling />
  <Nested />
  <HtmlTag />
  <Assignments />
  <Declarations />
  <Statements />
  <UpdateArray />
  <UpdateObject />
  <DeclaringProps />
  <DefaultProps />
  <SpreadProps />
  <IfBlocks />
  <ElseBlocks />
  <ElseIfBlocks />
  <EachBlock />
  <KeyedEachBlock />
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
