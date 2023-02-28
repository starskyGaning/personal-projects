<script>
    export let destLink;
    export let destName = 'Link';
</script>

<li class="nav-item">
    <a href="{destLink}" class="nav-link">{destName}</a>
</li>

<style lang="scss">
    @use '../../resources/scss/compiler' as c;

    .nav-link{
        @include c.heading-3;
        color: c.$secondary-500;
        transition: all 800ms ease;
    }
    .nav-link:hover{
        color: c.$secondary-300;
    }
</style>