<script>
    import SocialLink from "../../../components/footer/social-link.svelte";
</script>

<footer class="container-fluid">
    <div class="container d-flex flex-column flex-md-row align-items-baseline justify-content-between">
        <div class="d-flex flex-row align-items-center socials-row">
            <SocialLink bootIconName="bi-instagram"/>
            <SocialLink bootIconName="bi-youtube"/>
            <SocialLink bootIconName="bi-twitter"/>
        </div>
        <p>Copyright &copy; Emily Johnson, 2023, All Rights Reserved</p>
    </div>
</footer>

<style lang="scss">
    @use '../../scss/compiler' as c;

    footer{
        background-color: c.$secondary-500;
        color: c.$primary-500;
        .container{
            padding: 1.5rem 0;
        }
        .socials-row{
            gap: 1rem;
            margin-bottom: 1rem;
            @include c.MD{
                margin-bottom: 0;
            }
        }
    }
</style>