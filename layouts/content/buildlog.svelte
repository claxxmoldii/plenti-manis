<script>
  export let title, tagline, created;
</script>

<section class="buildLog container isGrid">
   <header>
      <h1>{ title }</h1>
      <h5>{ tagline }</h5>
  </header>

  <ul>
    <li>rebuild claxxmoldii from plenti --bare <span class="date">/2021.04.13</span></li>
    <li>switched to localhost:8888 <span class="date">/2021.04.13</span></li>
    <li>css... okay. <span class="date">/2021.04.13</span></li>
    <li>head... okay. <span class="date">/2021.04.13</span></li>
    <li>favicon... okay! <span class="date">/2021.04.13</span></li>
    <br>

    <li>collection endpoints seem okay <span class="date">/2021.04.13</span></li>
    <li>attributions & buildlog look, okay. <span class="date">/2021.04.13</span></li>
    <li>footer... okay <span class="date">/2021.04.13</span></li>
    <li>index... <span class="date">/2021.04.13</span></li>
    <li>about... okay <span class="date">/2021.04.13</span></li>
    <br>

    <li>rebuild, okay. <span class="date">/2021.04.13</span></li>
    <li>navigation seems okay but with issue: needs double-clicking on some links. consult js gurus... <span class="date">/2021.04.14</span></li>
    <li>now running on plenti v.4.16. yeah!</li>
    <li>maybe, consolidate everything into index... eh?</li>
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
