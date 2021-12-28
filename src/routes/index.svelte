<script>
    import SeoHead from '$lib/head.svelte'
    import Hero from '$lib/hero.svelte'
    import Projects from '$lib/projects.svelte'
    import HomeContent from '$lib/homeContent.svelte'
</script>

<SeoHead pageTitle="Home" />
<div class="home">
    <Hero />
    <Projects />
    <HomeContent />
</div>

<style>
    @import '../../static/styles/home.module.css';
</style>