<script>
  const user = {
    name: "No name yet",
  };

  function changeUserName() {
    user.name = "Oscar";
  }
</script>

<button on:click={changeUserName}>Change name to Oscar</button>
<p>{user.name}</p>
