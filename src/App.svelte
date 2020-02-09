<script>
  import Menu from "./components/Menu.svelte";
  import Footer from "./components/Footer.svelte";
  import Nav from "./components/Nav.svelte";
  import Page from "./components/Page.svelte";
  import Playlist from "./pages/Playlist.svelte";
</script>

<style>
  main {
    width: 100vw;
    height: 100vh;
    display: grid;
    grid-template-areas:
      "menu content"
      "footer footer";
    grid-template-rows: 1fr 96px;
    grid-template-columns: 200px 1fr;
  }
</style>

<main>
  <Menu />
  <Page>
    <Playlist />
  </Page>
  <Footer />
</main>
