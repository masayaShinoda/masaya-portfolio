<script>
  import Nav from '$lib/nav.svelte'
</script>

<Nav></Nav>
<main>
    <slot></slot>
</main>

<style>
  /* @import '/static/styles/globals.css'; */
  main {
    padding: 0 10%;
    margin: 5% auto;
    max-width: 1280px;
    /* border: 1px solid red; */
  }
  @media(max-width: 1023px) {
    main {padding: 10% 10%}
  }
  @media(max-width: 767px) {
    main {padding: 7.5% 7.5%}
  }
</style>