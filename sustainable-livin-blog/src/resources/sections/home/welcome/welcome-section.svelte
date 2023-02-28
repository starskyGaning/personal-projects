<script>
    import InputGroup from "../../../../components/home/welcome/input-group.svelte";
</script>

<section class="container-fluid welcome-section">
    <div class="container">
        <div class="row row-cols-1 row-cols-lg-2 align-items-center">
            <div class="d-flex flex-column col left-column">
                <h1>Welcome to Sustainable Livin</h1>
                <div class="d-flex flex-column welcome-text-box">
                    <p>We’ll provide you with knowledge on how to live a sustainable life</p>
                    <p>Subscribe to our newsletter so you never miss on the latest blog post</p>
                </div>
                <InputGroup />
            </div>
            <div class="d-flex flex-column align-items-center order-first order-lg-last col right-column">
                <img src="/illustrations/tree.svg" alt="tree-illustration" class="img-fluid">
            </div>
        </div>
    </div>
</section>

<style lang="scss">
    @use '../../../scss/compiler' as c;

    .welcome-section{
        background-color: c.$primary-500;
        .container{
            padding: 6rem 1rem;
            @include c.MD{
                padding: 6rem 0;
            }
            .left-column{
                h1{
                    @include c.display-1;
                    color: c.$secondary-900;
                    max-width: 700px;
                    margin-bottom: 2rem;
                }
                .welcome-text-box{
                    color: c.$secondary-500;
                    gap: 1rem;
                    margin-bottom: 2.5rem;
                    p{
                        @include c.heading-1;
                        max-width: 590px;
                    }
                }
            }
            .right-column{
                margin-bottom: 3rem;
                @include c.LG{
                    margin-bottom: 0;
                }
            }
        }
    }
</style>