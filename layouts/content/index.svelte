<script>
  import Navigation from '../components/navigation.svelte';

	export let title, tagline, current;
  // let pussySyrup = "annette";

  const tagNum = function (min, max) {
    min = Math.ceil(min);
    max = Math.floor(max);
    return Math.floor(Math.random() * (max - min + 1) + min); //The maximum is inclusive and the minimum is inclusive
}
</script>

<main class="isGrid">
  <section class="upperJones isGrid">
    <header class="isGrid">
      <div>
        <h1>{ title }</h1>
        <h3>{ tagline[tagNum(0,4)] }</h3>
      </div>

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
    /*margin-bottom: 10px;*/
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
  }

  h3 {
    font-size: 2rem;
    font-weight: 500;
    color: rgba(0, 0, 0, 0.5);
    margin: 0;
    margin-bottom:  10px;
  }
</style>
