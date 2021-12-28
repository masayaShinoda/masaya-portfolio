<script>
    import SeoHead from '$lib/head.svelte'
    import Hero from '$lib/hero.svelte'
    import Projects from '$lib/projects.svelte'
    import HomeContent from '$lib/homeContent.svelte'
</script>

<SeoHead pageTitle="Home" />
<main class="home">
    <Hero />
    <Projects />
    <HomeContent />
</main>

<style>
    @import '../../static/styles/home.module.css';
</style>