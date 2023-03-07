<script>
  import '../global.css';
</script>

<nav>
  <a href="/">Home</a>
  <a href="/posts">Posts</a>
  <a href="/favs">Favs</a>
  <a href="/info">Info</a>
  <a href="/about">About</a>
  <a href="/donate">Donate</a>
</nav>

<main>
  <slot />
</main>

<footer>
  <a href="/">&copy;2023 Eric York</a>
</footer>

<style>
  nav, footer {
    display: flex;
    justify-content: space-evenly;
    padding: .5em;
    background-color:honeydew;
    color: seagreen;
  }
  main {
    grid-row: 2;
    padding: 0 2rem;
    background-color: rgba(255,255,255,.05);
  }
  footer {
  grid-row: 3;
  position: sticky;
  bottom: 0;
  }
</style>