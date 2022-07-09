<script>
  import "../app.css";
  import NavBar from "$lib/components/nav-bar.svelte";
  import Footer from "$lib/components/footer.svelte";
</script>

<NavBar />

<main>
  <slot />
</main>

<Footer />

<!-- <style>
  :root {
    --bg-color: #ffffff;
    --text-color: #000000;
  }

  :global(body) {
    background: var(--bg-color);
    color: var(--text-color);
  }

  :global(body.dark) {
    --bg-color: #000000;
    --text-color: #ffffff;
  }
</style> -->
