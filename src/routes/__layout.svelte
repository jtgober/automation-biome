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
