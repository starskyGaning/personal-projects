<script>
    import Card from "../../../../components/home/blog-preview/card.svelte";
    import RedirectButton from "../../../../components/home/blog-preview/redirect-button.svelte";
</script>

<section class="container-fluid blog-preview-section">
    <div class="container">
        <div class="row row-cols-1 d-flex justify-content-center">
            <div class="col d-flex flex-column align-items-center header-sub-section">
                <h1>Blogs</h1>
            </div>
            <div class="col d-flex justify-content-center row row-cols-1 row-cols-lg-2 row-cols-xxl-3 cards-sub-section">
                <Card />
            </div>
            <div class="col d-flex justify-content-center">
                <RedirectButton  destRedirect="/blog/" destName="See More Blogs"/>
            </div>
        </div>
    </div>
</section>

<style lang="scss">
    @use '../../../scss/compiler' as c;

    .blog-preview-section{
        background-color: c.$primary-500;
        .container{
            padding: 5rem 1rem;
            @include c.LG{
                padding: 5rem 0;
            }
            .header-sub-section{
                margin-bottom: 5rem;
                h1{
                    @include c.display-2;
                }
            }
            .cards-sub-section{
                margin-bottom: 3.5rem;
            }
        }
    }
</style>