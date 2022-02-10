<script>
    import SvelteMarkdown from 'svelte-markdown'
    const portfMdWeb =
`
- 
[
![screenshot of Good Time Hospitality Group website](/images/1280w/gt-rr-mockup-laptop-phone_result.png)
Hospitality & Resort Website
](https://goodtimehospitality.com/)
- 
[
![screenshot of Zillion United's corporate website](/images/1280w/z1-corporate_result.png)
Trading App Corporate Website
](https://zillionunited.io)
- 
[
![screenshot of blog.masayashida.com](/images/1280w/masayas-thoughts_result.png)
Personal blog website
](https://blog.masayashida.com)
-
[
![screenshot of cryptocalc-site.vercel.app](/images/1280w/cryptocalc_result.png)
Cryptocurrency investment calculator
](https://cryptocalc-site.vercel.app/)
-
[
![screenshot of sentinelspropertyalliance.com](/images/1280w/sentinelsproperty_result.png)
Real estate listings website
](https://sentinelspropertyalliance.com)
-
[
![screenshot of Masaya's FreeCodeCamp certificate](/images/1x/fcc-certif.png)
FCC Certification projects
](https://fcc.masayashida.com)
`

</script>
<section class="projectsSection" id="projects">
    <h2>Projects</h2>
    <!-- <h3>Web Design & Development</h3> -->
    <SvelteMarkdown source={portfMdWeb} />
</section>

<style>
    @import '../../static/styles/projects.module.css';
</style>