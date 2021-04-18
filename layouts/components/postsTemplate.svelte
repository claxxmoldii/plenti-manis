<script>
  export let title, byline, body;
</script>

<main class="">
  <h3>{ title }/</h3>  
  <h4>{ byline }</h4>
  <p>{@html body}</p>
    
</main>

<style>
  p {
    display: block;
  }
</style>
