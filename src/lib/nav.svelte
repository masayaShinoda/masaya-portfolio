<script>
    let mobileNavOpened = false
    function handleMobileNav() {
        if(mobileNavOpened) {
            document.getElementsByTagName("body")[0].style.height = "auto"
            document.getElementsByTagName("body")[0].style.overflowY = "initial"            
        } else {
            document.getElementsByTagName("body")[0].style.height = "100%"
            document.getElementsByTagName("body")[0].style.overflowY = "hidden" //disable mobile scroll
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
        <img src="/images/SVG/masaya-web-dev-logo.svg" alt="Logo" class="mainLogo">
        <img src="/images/SVG/maya-logo-vert.svg" alt="logo" class="mobileLogo">
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
    <nav id="nav">
        <ul on:click={handleMobileNav}>
            <li>
                <a href="https://github.com/masayaShinoda">Projects</a>
            </li>
            <li>
                <a href="https://www.linkedin.com/in/masaya-shida/">Contact</a>
            </li>
            <li id="home_link">
                <a href="/">Home</a>
            </li>
            <!-- <li>
                <a href="/" lang="khm">ភាសាខ្មែរ</a>
            </li> -->
        </ul>
    </nav>
</div>

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