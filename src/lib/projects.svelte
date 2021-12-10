<script>
    import SvelteMarkdown from 'svelte-markdown'
    const portfMd =
`
- 
[
![screenshot of blog.masayashida.com](/images/1280w/masayas-thoughts_result.png)
Personal blog website
](https://github.com/masayaShinoda/masayas-thoughts-site)
-
[
![screenshot of cryptocalc-site.vercel.app](/images/1280w/cryptocalc_result.png)
Cryptocurrency investment calculator
](https://github.com/masayaShinoda/cryptocalc-site)
-
[
![screenshot of FreeCodeCamp certificate](/images/1x/fcc-certif.png)
FCC Certification projects
](https://fcc.masayashida.com)
`

</script>
<section class="projectsSection" id="projects">
    <h2>Projects</h2>
    <SvelteMarkdown source={portfMd} />
</section>



<style>
    @import '../../static/styles/projects.module.css';
</style>