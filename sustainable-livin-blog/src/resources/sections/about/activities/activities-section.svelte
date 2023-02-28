<script>
</script>

<section class="container-fluid activities-section">
    <div class="container">
        <div class="row row-cols-1">
            <div class="col">
                <h1>Favorite activities</h1>
                <p>When I'm not conducting research, you can usually find me hiking, bird watching, or reading up on the latest scientific findings in my field.</p>
            </div>
        </div>
    </div>
</section>

<style lang="scss">
    @use '../../../scss/compiler' as c;

    .activities-section{
        background-color: c.$primary-500;
        .container{
            padding: 5rem 1rem;
            @include c.MD{
                padding: 8rem 0;
            }
            h1{
                @include c.display-3;
                color: c.$secondary-500;
                text-decoration: underline;
                margin-bottom: 2rem;
            }
            p{
                @include c.heading-1;
                color: c.$secondary-400;
                max-width: 990px;
            }
        }
    }
</style>