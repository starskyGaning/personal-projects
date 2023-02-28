<script>
    import Card from "../../../../components/home/blog-preview/card.svelte";
</script>

<section class="container-fluid blogs-section">
    <div class="container">
        <div class="row row-cols-1 row-cols-lg-2 row-cols-xxl-3">
            <Card />
        </div>
    </div>
</section>

<style lang="scss">
    @use '../../../scss/compiler' as c;

    .blogs-section{
        background-color: c.$primary-500;
        .container{
            padding: 4rem 1rem;
            @include c.MD{
                padding: 6rem 0;
            }
        }
    }
</style>