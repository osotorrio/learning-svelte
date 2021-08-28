<script>
  let players = [
    { id: 1, name: "Raul Capablanca", elo: 2600 },
    { id: 2, name: "Anatoly Karpov", elo: 2700 },
    { id: 3, name: "Magnus Carlsen", elo: 2800 },
    { id: 4, name: "Bobby Fischer", elo: 2800 },
    { id: 5, name: "Garray Kasparov", elo: 2800 },
  ];

  function removeFirstPlayer() {
    players = players.splice(1);
  }
</script>

<div id="keyed-each-blocks">
  <button on:click={removeFirstPlayer}>Remove first player</button>
  <ul>
    {#each players as player (player.id)}
      <li title="Elo: {player.elo}">{player.name}</li>
    {/each}
  </ul>
  <hr />
</div>
