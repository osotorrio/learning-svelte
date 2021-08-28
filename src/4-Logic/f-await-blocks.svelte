<script>
  let shouldFail = false;

  function fakeCall() {
    return new Promise((resolve, rejected) => {
      setTimeout(() => {
        shouldFail
          ? rejected("Something went wrong!!")
          : resolve("Fake message from the server ;)");
        shouldFail = true;
      }, 3000);
    });
  }

  function makeLongCall() {
    promise = fakeCall();
  }

  let promise = fakeCall();
</script>

<div id="await-blocks">
  <button on:click={makeLongCall}>Click to make call that fails</button>

  {#await promise}
    <p>waiting for the server...</p>
  {:then message}
    <h2>{message}</h2>
  {:catch error}
    <p class="red-error">{error}</p>
  {/await}

  <hr />
</div>

<style>
  .red-error {
    color: red;
  }
</style>
