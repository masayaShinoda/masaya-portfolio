<script>
    import AnnouncementBanner from '$lib/announcementBanner.svelte'

    let mobileNavOpened = false
    function handleMobileNav() {
        if(mobileNavOpened) {
            document.getElementsByTagName("body")[0].style.height = "auto"
            document.getElementsByTagName("body")[0].style.overflowY = "initial"
        } else {
            
            document.getElementsByTagName("body")[0].style.height = "100%"
            document.getElementsByTagName("body")[0].style.overflowY = "hidden" //disable mobile scroll
            // scroll to top to prevent tearing
            document.body.scrollTop = 0;
            document.documentElement.scrollTop = 0;
        }
        mobileNavOpened = !mobileNavOpened
        document.getElementById("nav").classList.toggle("active")        
        handleMobileNavBtn()

    }
    function handleMobileNavBtn() {
        document.getElementById("mobileNavBtn").classList.toggle("close")
    }

</script>

<div class="navContainer">
    <a href="/">
        <img src="/images/SVG/masaya-web-dev-logo.svg" alt="Masaya Shida logo" class="mainLogo">
        <img src="/images/SVG/maya-logo-vert.svg" alt="Masaya Shida logo" class="mobileLogo">
    </a>
    <button
        on:click={handleMobileNav} 
        class="mobileNavBtn"
        id="mobileNavBtn"
    >
        <span></span>
        <span></span>
        <span></span>
    </button>
    <!-- svelte-ignore a11y-no-redundant-roles -->
    <nav id="nav" role="navigation">
        <ul on:click={handleMobileNav}>
            <li>
                <a href="/#projects">Projects</a>
            </li>
            <li>
                <a href="/contact">Contact</a>
            </li>
            <li id="home_link">
                <a href="/">Home</a>
            </li>
            <!-- <li>
               <a 
               href="https://courses-kh.masayashida.com/"
               lang="km"
               >
                វគ្គសិក្សា
                </a> 
            </li> -->
            <!-- <li>
                <a href="/" lang="khm">ភាសាខ្មែរ</a>
            </li> -->
        </ul>
    </nav>
</div>
<AnnouncementBanner />

<style>
    @import '../../static/styles/nav.module.css';
    ul {
        display: flex;
        list-style-type: none;
        margin: 0;
    }
    li {
        line-height: 1;
    }

</style>