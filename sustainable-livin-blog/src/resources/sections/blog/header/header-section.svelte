<script>

</script>

<section class="container-fluid header-section">
    <div class="container">
        <h1>Welcome to the Blog Page</h1>
        <h2>You’ll get a highly curated blog posts about how to live a sustainable life</h2>
    </div>
</section>

<style lang="scss">
    @use '../../../scss/compiler' as c;

    .header-section{
        background-color: c.$primary-500;
        .container{
            padding: 3rem 1rem;
            @include c.MD{
                padding: 3rem 0;
            }
            h1{
                @include c.display-1;
                margin-bottom: 2rem;
            }
            h2{
                @include c.heading-1;
                max-width: 620px;
            }
        }
    }
</style>