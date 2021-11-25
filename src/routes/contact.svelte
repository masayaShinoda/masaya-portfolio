<script>
    import SeoHead from '$lib/head.svelte'
</script>

<SeoHead pageTitle="Contact" />
<div class="contactContainer">
    <section class="aboutContainer">
        <h1>Contact me</h1>
        <span class="socials">
            <a href="https://www.linkedin.com/in/masaya-shida/">
                LinkedIn
            </a>
            <a href="https://github.com/masayaShinoda">
                GitHub
            </a>
            <a href="https://t.me/shinoda17">
                Telegram
            </a>        
        </span>
    </section>
    <section class="formContainer">
        <form
            action="https://formspree.io/f/xrgjzevq"
            method="POST"
        >
            <span class="namesSpan">
                <label for="fname">
                    First name:
                    <input type="text" id="fname" name="fname"><br>
                </label>
                <label for="lname">
                    Last name:
                    <input type="text" id="lname" name="lname"><br>
                </label>

            </span>
            <label>
                Email:
                <input type="email" name="_replyto">
            </label>
            <label>
                Message:
                <textarea name="message" wrap="off"></textarea>
            </label>
            <button type="submit">Send message</button>
        </form>
    </section>
</div>

<style>
    @import '../../static/styles/contact.module.css';
</style>