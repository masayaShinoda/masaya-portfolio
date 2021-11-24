<script>
  import Nav from '$lib/nav.svelte'
</script>

<Nav></Nav>
<main>
    <slot />
</main>

<style>
    @import '../../static/styles/layout.module.css';

  main {
    /* padding: 10% 0; */
    margin: 0 auto;
  }
</style>