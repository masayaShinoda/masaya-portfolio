<script>
  export let pageTitle;
</script>

<svelte:head>
    <!-- head content -->
      {#if pageTitle}
        <title>{pageTitle} | Masaya Shida</title>
        {:else}
        <title>Masaya Shida | Cambodia-based Web Developer</title>
      {/if}
      
      <link rel="stylesheet" href="/styles/reset.css">
      <link rel="stylesheet" href="/styles/globals.css">
      
      <meta name="description" content="Cambodia-based web developer and graphic designer.">
      <meta name="keywords" content="masayashida, masaya shida, shida masaya, masaya shida portfolio, works by masaya shida">
  
      <!-- Open Graph / Facebook -->
      <meta property="og:type" content="website">
      <meta property="og:title" content="Masaya Shida">
      <meta property="og:description" content="Cambodia-based web developer and graphic designer.">
      <meta property="og:image" content="images/1024w/banner-logo-margins.png">
  
      <!-- Twitter -->
      <meta property="twitter:card" content="summary_large_image">
      <meta property="twitter:title" content="Masaya Shida">
      <meta property="twitter:description" content="Cambodia-based web developer and graphic designer.">
      <meta property="twitter:image" content="images/1024w/banner-logo-margins.png">
  
  </svelte:head>