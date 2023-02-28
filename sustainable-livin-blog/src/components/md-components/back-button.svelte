<script>
    export let backDest = "/blog/";
    export let backName = "Back";
</script>

<a href="{backDest}">{backName}</a>

<style lang="scss">
    @use '../../resources/scss/compiler' as c;

    a{
        @include c.heading-3;
        background-color: c.$secondary-500;
        color: c.$primary-500;
        text-decoration: none;
        padding: 1.5rem 3rem;
        transition: all 800ms ease;
    }
    a:hover{
        background-color: c.$primary-500;
        color: c.$secondary-500;
    }
</style>