<script>
  export let title, tagline;
</script>

<main class="isFlex">
  <div class="titleBar">
    <h3>{ title }/</h3>
  </div>
  <ul>
    <h4>{ tagline }</h4>
    
    <li><a href="https://nodejs.org/en/">https://<span>nodejs</span>.org/en/</a></li>
    <li><a href="https://www.npmjs.com/">https://www.<span>npmjs</span>.com/</a></li>
    <li><a href="https://brew.sh/">https://<span>homebrew</span>.sh/</a></li>
    <li><a href="https://www.snowpack.dev/">https://www.<span>snowpack</span>.dev/</a></li>
    <li><a href="https://rollupjs.org/guide/en/">https://<span>rollupjs</span>.org/guide/en/</a></li>
    <li><a href="https://firebase.google.com/">https://<span>firebase</span>.google.com/</a></li>
    <li><a href="https://aws.amazon.com/">https://<span>aws</span>.amazon.com/</a></li>
  </ul>
</main>

<style>
  .titleBar {
    width: 300px;
  }

  h3 {
    font-weight:  400;
    /*display: inline;*/
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
    display:  inline;
  }
</style>
