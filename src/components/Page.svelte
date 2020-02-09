<script>
  import Nav from "./Nav.svelte";
</script>

<style>
  section {
    grid-area: content;
    background: linear-gradient(45deg, #222, #181818);
    display: flex;
    flex-direction: column;
  }
</style>

<section>
  <Nav />
  <slot />
</section>
