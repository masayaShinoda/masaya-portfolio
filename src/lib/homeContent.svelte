<script>
    import SvelteMarkdown from 'svelte-markdown'

    const contentSection1 =
`
## Design Philosophy: Minimal & Practical 
I believe that in this busy world, we tend to overlook how important it is to keep things simple and clutterless. My design approach is to deliver essential information in an easy-to-read manner, and speedy websites with straightforward navigation.
`
</script>

<section class="content_sections_container">
    <div class="content_section">
        <span>
            <SvelteMarkdown source={contentSection1} />
        </span>
        <img src="/images/SVG/golden-ratio.svg" alt="golden ratio spiral">
    </div>
</section>