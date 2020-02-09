<script>
  import user from "../stores/user";
</script>

<style lang="scss">
  nav {
    height: 64px;
    display: flex;
  }

  .navigation {
    display: flex;
    align-items: center;
    justify-items: center;
    margin-left: 8px;

    svg {
      width: 28px;
    }
  }

  form {
    flex-grow: 1;
    display: flex;
    align-items: center;
    margin-left: 8px;

    input {
      color: #333;
      border-radius: 20px;
      height: 40px;
      border: none;
      font-size: 12px;
      padding: 16px;
      min-width: 246px;
    }
  }

  .user {
    display: flex;
    margin-right: 16px;
    align-items: center;
    justify-content: center;

    img {
      border-radius: 50%;
      margin-right: 8px;
      width: 36px;
    }
  }
</style>

<nav>
  <aside class="navigation">
    <svg viewBox="0 0 24 24" class="prev">
      <path fill="currentColor" d="M15.54 21.15L5.095 12.23 15.54 3.31l.65.76-9.555 8.16 9.555 8.16" />
    </svg>
    <svg viewBox="0 0 24 24" class="next">
      <path fill="currentColor" d="M7.96 21.15l-.65-.76 9.555-8.16L7.31 4.07l.65-.76 10.445 8.92" />
    </svg>
  </aside>
  <form>
    <input placeholder="Search for songs, artists or podcasts" type="text" />
  </form>
  {#if user}
    <aside class="user">
      <img src={user.avatar} alt={user.name} />
      <span>{user.name}</span>
    </aside>
  {/if}
</nav>
