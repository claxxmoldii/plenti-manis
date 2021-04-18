<script>
  import Navigation from '../components/navigation.svelte';

  export let title, tagline, current;
</script>

<main class="isGrid">
  <section class="upperJones isGrid">
    <header class="isGrid">
      <h1>{title}</h1>
    </header>
  </section>

  <section class="lowerJones isGrid">
    <div class="isNav isGrid">
      <Navigation {current}/>
    </div>
  </section>
</main>

<style>
  main {
    max-width: 50vw;
    max-height: 100vh;
    margin-left: 30vw;
    grid-template-rows: 40vh auto;
  }

  section {
    width: 50vw;
    margin: 0;
  }

  header {
    border-bottom: 2px solid #ff6565;
    align-items: end;
  }

  .isNav {
    justify-items: end;
    margin-top: 10px;
  }

  h1 {
    font-size: 3rem;
    font-weight: 500;
    letter-spacing: 1px;
    margin: 0;
    margin-bottom: 10px;
  }

  h3 {
    font-size: 2rem;
    font-weight: 500;
    color: rgba(0, 0, 0, 0.5);
  }
</style>
