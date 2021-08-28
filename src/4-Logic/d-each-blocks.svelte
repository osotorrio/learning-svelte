<script>
  const players = [
    { name: "Raul Capablanca", elo: 2600 },
    { name: "Anatoly Karpov", elo: 2700 },
    { name: "Magnus Carlsen", elo: 2800 },
  ];
</script>

<div id="each-blocks">
  <ul>
    {#each players as { name, elo }, index}
      <li title="Elo: {elo}">{index + 1} {name}</li>
    {/each}
  </ul>
  <hr />
</div>
