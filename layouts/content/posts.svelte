<script>
  import Navigation from '../components/navigation.svelte';
  import PostsTemplate from '../components/postsTemplate.svelte';

  export let components, allLayouts, content, allContent;
  export let title, tagline, component, current, byline, body;

  let allCollections = allContent.filter(content => content.type == "collections");
</script>

<main class="isGrid">
  <section class="upperJones isGrid">
    <header class="isGrid">
      <h1>posts</h1>
    </header>
  </section>

  <section class="lowerJones">
    <div class="isNav">
      <Navigation {current}/>
    </div>

    <PostsTemplate {title} {byline} {body}/>


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

  .lowerJones {
    display:  flex;
    flex-direction: column;
  }

  header {
    border-bottom: 2px solid #ff6565;
    align-items: end;
  }

  .isNav {
    align-self: flex-end;
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

  a {
    text-decoration: none;
    color: rgba(220, 20, 60, 0.4);
  }

  a:hover {
    color: indianred;
  }

  li {
    list-style: none;
    color:  dimgray;
    display: inline;
  }

  .collection {
    margin: 0;
  }
</style>
