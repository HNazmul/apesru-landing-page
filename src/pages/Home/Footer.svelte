<script lang="ts">
    import IMG_FOOTER_BG from "../../assets/images/footer-background.png";
    import LOGO_APESRU from "../../assets/images/logo.png";

    const footerLinks = [
        {
            label: "OpenSea",
            link: "https://opensea.io/collection/katun-apes-r-us",
        },
        {
            label: "Twitter",
            link: "https://twitter.com/ApesRus_io",
        },
        {
            label: "Discord",
            link: "https://discord.com/invite/apesrus",
        },
    ];
</script>

<footer id="footer" class="theme-border border-top" style="--bg-img:url({IMG_FOOTER_BG})">
    <div class="footer-area">
        <div class="footer-container container-2k">
            <div class="row py-5 align-items-center w-100">
                <div class="col-lg-6 text-center">
                    <img src="{LOGO_APESRU}" class="footer-logo" alt="" />
                </div>
                <div class="col-lg-6">
                    <ul class="nav footers-links justify-content-center justify-content-lg-end align-items-center">
                        {#each footerLinks as link}
                            <li class="nav-item">
                                <a class="nav-link active" target="_blank" href="{link.link}">{link.label}</a>
                            </li>
                        {/each}
                    </ul>
                </div>
            </div>
        </div>
    </div>
</footer>

<style lang="scss">
    @use "../../styles/pageHome" as main;
    @include main.footer();
</style>
