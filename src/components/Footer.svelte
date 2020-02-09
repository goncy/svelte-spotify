<script>
  import song from "../stores/playing";
</script>

<style lang="scss">
  footer {
    grid-area: footer;
    background-color: #282828;
    display: flex;
  }

  .song {
    width: 200px;
    padding: 16px;
    display: flex;
    flex-direction: column;
    justify-content: center;

    .title {
      font-size: 16px;
      color: white;
    }

    .author {
      font-size: 12px;
      color: #999;
    }
  }

  section {
    display: flex;
    align-items: center;
    flex-grow: 1;
    padding: 16px;
  }

  .controls {
    padding: 16px;
    display: flex;
    align-items: center;
  }
</style>

<footer>
  <aside class="song">
    <div class="title">{song.title}</div>
    <div class="author">{song.author}</div>
  </aside>
  <section>Player</section>
  <aside class="controls">Controls</aside>
</footer>
