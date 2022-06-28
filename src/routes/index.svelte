<script>
  let title = "what a ham";

  const updateTitle = () => {
    title = "updated title";
  };
</script>

<div class="index">
  <h1>{title}</h1>
  <p>
    This is a test endpoint that can be accessed <a href="/about">HERE!!</a> :)
  </p>
  <button on:click={updateTitle}>Update title</button>
  <input type="text" class="textArea" bind:value={title} />
</div>

<style>
  .index {
    color: purple;
    text-align: center;
    display: block;
    font-family: "Comic Sans MS", cursive;
    font-size: 2em;
  }
</style>
