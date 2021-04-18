<script>
  import Head from './head.svelte';
  import Footer from './footer.svelte';

  export let content, layout, allContent;
</script>

<html lang="en">
<Head title={content.filename} />

<body class="isGrid">
  <svelte:component this={layout} {...content.fields} {allContent} />

  <footer class="isFlexCentered">
    <Footer />
  </footer>
</body>
</html>

<style>
  body {
    height: 100vh;
    grid-template-rows: auto 30px;
  }
</style>
