<script>
</script>

<section class="container-fluid bio-section">
    <div class="container">
        <div class="row row-cols-1 row-cols-md-2 justify-content-center">
            <div class="col d-flex flex-column left-column">
                <h1>Emily Johnson</h1>
                <h2>Nature Researcher</h2>
                <p>Hi there! I'm Emily, a nature researcher with a passion for exploring and learning about the natural world. I'm excited to share my findings and insights with you through my blog. Join me on my journey as I explore the wonders of nature!</p>
            </div>
            <div class="col d-flex flex-column align-items-center order-first order-md-last right-column">
                <img src="/profile/profile.png" alt="portrait" class="img-fluid">
            </div>
        </div>
    </div>
</section>

<style lang="scss">
    @use '../../../scss/compiler' as c;

    .bio-section{
        background-color: c.$primary-500;
        .container{
            padding: 5rem 1rem;
            @include c.MD{
                padding: 7rem 0;
            }
            .left-column{
                h1{
                    @include c.display-2;
                    color: c.$secondary-500;
                    margin-bottom: .5rem
                }
                h2{
                    @include c.heading-2;
                    color: c.$secondary-400;
                    margin-bottom: 2rem;
                }
                p{
                    @include c.heading-3;
                    color: c.$secondary-900;
                    max-width: 750px;
                }
            }
            .right-column{
                margin-bottom: 3rem;
                @include c.MD{
                    margin-bottom: 0;
                }
                img{
                    max-width: 300px;
                }
            }
        }
    }
</style>