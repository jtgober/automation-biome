<script>

  let darkMode = false;
  function toggle() {
    darkMode = !darkMode;
    window.document.body.classList.toggle("dark");
  }
</script>

<button on:click={toggle}>
  {#if darkMode}
  <img class=" object-contain h-6 w-6 md:hover:bg-slate-500 rounded-full object-center" src="./sunny-outline.png" alt="">
  {:else}
 <img class=" object-contain h-6 w-6 md:hover:bg-gray-200 rounded-full object-center" src="./moon-outline.png" alt="">
  {/if}
</button>


