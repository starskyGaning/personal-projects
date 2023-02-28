<script>
    export let destRedirect = "/";
    export let destName = "Link";
</script>

<a href="{destRedirect}">{destName}</a>

<style lang="scss">
    @use '../../../resources/scss/compiler' as c;

    a{
        @include c.heading-3;
        text-decoration: none;
        background-color: c.$secondary-500;
        color: c.$primary-500;
        padding: 1.5rem 5rem;
        transition: all 800ms ease;
    }
    a:hover{
        background-color: c.$primary-500;
        color: c.$secondary-500;
    }
</style>