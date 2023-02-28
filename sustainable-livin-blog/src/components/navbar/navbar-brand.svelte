<script>
    export let dest;
</script>

<a href="{dest}" class="navbar-brand">
    <img src="/logo/logo.svg" alt="blog-page-logo">
</a>

<style lang="scss">
    @use '../../resources/scss/compiler' as c;

    a{
        img{
            width: 3rem;
            transition: all 800ms ease;
        }
    }
    a:hover{
        img{
            transform: scale(1.5);
        }
    }


</style>