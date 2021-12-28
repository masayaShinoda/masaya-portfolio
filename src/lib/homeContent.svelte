<script>
    import SvelteMarkdown from 'svelte-markdown'

    const contentSection1 =
`
## Design Philosophy - Minimal & Practical
I believe that in this busy world, we tend to overlook how important it is to keep things simple and clutterless. My design approach is to deliver essential information in an easy-to-read manner, and make webpages fast with navigation that is as straightforward as possible.

`
</script>

<section class="content_sections_container">
    <div class="content_section">
        <span>
            <SvelteMarkdown source={contentSection1} />
        </span>
    </div>
</section>
