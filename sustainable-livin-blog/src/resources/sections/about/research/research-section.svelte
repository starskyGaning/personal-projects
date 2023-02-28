<script>
</script>

<section class="container-fluid research-section">
    <div class="container">
        <div class="row row-cols-1">
            <div class="col">
                <h1>Research Focus</h1>
                <p>My research focuses on the ecology of forest ecosystems, particularly the interactions between plants and animals. I'm interested in understanding how these ecosystems function and how we can better conserve them.</p>
            </div>
        </div>
    </div>
</section>

<style lang="scss">
    @use '../../../scss/compiler' as c;

    .research-section{
        background-color: c.$primary-500;
        .container{
            padding: 5rem 1rem;
            @include c.MD{
                padding: 10rem 0;
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
                max-width: 1050px;

            }
        }
    }
</style>