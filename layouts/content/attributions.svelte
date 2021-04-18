<script>
  export let title, tagline, created;
</script>

<section class="attributions container isGrid">
  <header>
    <h1>{ title }</h1>
    <h5>{ tagline }</h5>
  </header>
  <ul>
    <li>plenti</li>
    <li>svelte</li>
    <li>skeleton css</li>
    <li>google font/raleway</li>
    <li>manis/yurizal susanto</li>
  </ul>
</section>

<style>
  .container {
    width:  50vw;
  }

  .attributions {
    margin-top:  30vh;

    /*background-color:  beige;*/
    grid-template-columns: 1fr 1fr;
    grid-template-areas: "title list";
  }

  header {
    grid-area: title;
  }

  ul {
    grid-area: list;
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
