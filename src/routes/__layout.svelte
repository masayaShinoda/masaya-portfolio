<script>
  import Nav from '$lib/nav.svelte'
</script>

<Nav></Nav>
<main>
    <slot />
</main>

<style>
  main {
    /* padding: 10% 0; */
    margin: 0 auto;
  }
</style>