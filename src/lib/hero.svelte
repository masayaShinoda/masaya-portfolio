<script>
    import SvelteMarkdown from 'svelte-markdown'

    const heroMd =
`
# Cambodia-based Web Developer
Hello! My name is Masaya and I help businesses and ideas achieve a quality online presence.

[See my projects](#projects)
`
</script>

<section class="hero">
    <span>
        <SvelteMarkdown source={heroMd} />
    </span>
    <img src="/images/1x/hero-mockup.png" alt="Website mockups">
</section>
<section class="skillset">
    <h2>Skillset</h2>
    <div>
        <img 
            src="/images/SVG/technologies-list.svg" 
            alt="Logos of HTML & CSS, JavaScript, ReactJS, NextJS, SvelteJS, Bootstrap"
        />
    </div>
</section>

<style>
    @import '../../static/styles/hero.module.css';
</style>