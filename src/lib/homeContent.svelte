<script>
    import SvelteMarkdown from 'svelte-markdown'

    const contentSections =
[
{
    content:
`
## Design Philosophy: Minimal & Practical 
I believe that in this busy world, we tend to overlook how important it is to keep things simple and clutterless. My design approach is to deliver essential information in an easy-to-read manner, and speedy websites with straightforward navigation.
`,
    image:  
{
    src: "/images/SVG/golden-ratio.svg",
    alt: "illustration of golden ratio spiral"
}
},
{
    content:
`
## Accessibility as a necessity
Since the web is a platform that is accessed by a wide variety of devices, and by people with physical or cognitive challenges, it matters to me that webpages pass essential [WCAG](https://www.w3.org/WAI/WCAG21/quickref/) standards such as perceivability, distinguishability, and operability in order to try to be as accessible as possible.
`,
    image:
{
    src: "/images/SVG/accessibility-icon.svg",
    alt: "illustration of touchscreen interaction"
}
}
]


</script>

<section class="content_sections_container">
    <div class="content_section">
        {#if contentSections}
        {#each contentSections as section}
            <span>
                <SvelteMarkdown source={section[`content`]} />
                {#if section['image']}
                    <img src={section['image']['src']} alt={section['image']['alt']} />
                {/if}
            </span>
        {/each}
        {/if}
        <span>
        </span>
    </div>
</section>