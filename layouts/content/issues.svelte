<script>
  export let title, tagline, created;
</script>

<section class="buildLog container isGrid">
   <header>
      <h1>{ title }</h1>
      <h5>{ tagline }</h5>
  </header>

  <ul>
    <li>
      navigation.svelte is based on svelte class directive 'https://svelte.dev/tutorial/classes'. it's wonky here. [collections] and [about] links have to be double-clicked for css to take effect. links are working though. [home] and [posts] are okay.
      resolved. svelte prop passing. <span class="date">/2021.04.17</span>
    </li>
    <br>

    <li>
      links... have to be refreshed. i'm not sure what's going on here but after watcing jantcu/plenti bigspring: part 18 video, tried turning off javascript, and funky stuff went away. tried running public folder on npm-http-server, links need refreshing. turned off js, funky stuff went away. using FF. tried it on brave, same thing...
    </li>

  </ul>
</section>

<style>
  .container {
    width:  50vw;
  }

  .buildLog {
    margin-top: 30vh;

    /*background-color:  beige;*/
    grid-template-columns: 1fr 1fr;
    grid-template-areas: "title list";
  }

  .title {
    grid-area: title;
  }

  ul {
    grid-area: list;
    padding-bottom: 100px;
  }

  li {
    font-size: 1.6rem;
    list-style: none;
  }

  .date {
    color: lightskyblue;
    padding-left:  10px;
  }
</style>
