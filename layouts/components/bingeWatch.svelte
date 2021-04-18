<script>
  export let title, tagline;
</script>

<main class="isFlex">
  <div class="titleBar">
    <h3>{ title }/</h3>
    <br>
  </div>
  <ul>
    <h4>{ tagline }</h4>
      <li><a href="https://www.youtube.com/channel/UCZSr5B0l07JXK2FIeWA0-jw/videos">
        sveltesociety</a>
      </li>
      <li><a href="https://www.youtube.com/watch?v=vEQhLyqgFE4">sveltemastery</a></li>
      <li><a href="https://www.youtube.com/channel/UCSJbGtTlrDami-tDGPUV9-w">
        academind</a>
      </li>
      <li><a href="https://www.youtube.com/channel/UCW5YeuERMmlnqo4oq8vwUpg">
        netninja</a>
      </li>
      <li><a href="https://www.youtube.com/channel/UCLNgu_OupwoeESgtab33CCw">
        codinggarden</a>
      </li>
      <li><a href="https://www.youtube.com/channel/UCJZv4d5rbIKd4QHMPkcABCw">
        kevinpowell</a>
      </li>
      <li><a href="https://www.youtube.com/channel/UCyOXWTxea5FbOcyIjbB9SvA">
        jantcu</a>
      </li>
  </ul>
</main>

<style>
  .titleBar {
    width: 300px;
  }

  h3 {
    font-weight: 400;
    display: inline;
    font-size:  2rem;
  }

  h4 {
    display: inline;
    font-size:  1.7rem;
  }

  span {
    color: indianred;
  }

    a {
    text-decoration: none;
    color: rgba(220, 20, 60, 0.4);
  }

  a:hover {
    color: indianred;
  }

  ul {
    margin-left: 30px;
  }

  li {
    line-height: 1rem;
    list-style: none;
    color:  dimgray;
    display:  inline-block;
  }
</style>
