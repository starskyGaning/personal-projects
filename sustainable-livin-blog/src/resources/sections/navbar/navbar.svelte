<script>
    import NavbarBrand from "../../../components/navbar/navbar-brand.svelte";
    import NavbarLink from "../../../components/navbar/navbar-link.svelte";
</script>

<nav class="container-fluid navbar navbar-expand-lg">
    <div class="container">
      <NavbarBrand dest="/"/>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <NavbarLink destLink="/about/" destName="About Me"/>
          <NavbarLink destLink="/blog/" destName="Blogs"/>
        </ul>
      </div>
    </div>
</nav>

<style lang="scss">
    @use '../../scss/compiler' as c;

    nav{
        background-color: c.$primary-500;
        .container{
            padding: 1rem;
            @include c.LG{
                padding: 1rem 0;
            }
        }
    }
</style>