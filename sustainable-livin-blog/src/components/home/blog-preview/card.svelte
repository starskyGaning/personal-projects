<script>
    import card from '../../../resources/json/card.json';
</script>

{#each card as {title,text,image,link} }
    <div class="col d-flex justify-content-center card-col">
        <figure class="position-relative">
            <!-- svelte-ignore a11y-img-redundant-alt -->
            <img src="{image}" alt="some-image">
            <figcaption class="position-absolute">
                <h1>{title}</h1>
                <p>{text}</p>
                <a href="{link}">See More</a>
            </figcaption>
        </figure>
    </div>
{/each}


<style lang="scss">
    @use '../../../resources/scss/compiler' as c;

    figure{
        img{
            max-width: 422px;
        }
        figcaption{
            left: 1rem;
            bottom: 1rem;
            padding: .5rem;
            h1{
                @include c.heading-3;
                color: c.$primary-500;
            }
            p{
                @include c.body;
                color: c.$primary-300;
                margin-bottom: 2rem;
            }
            a{
                @include c.body;
                text-decoration: none;
                background-color: c.$secondary-500;
                color: c.$primary-500;
                padding: 1rem 1.5rem;
                transition: all 800ms ease;
            }
            a:hover{
                background-color: c.$primary-500;
                color: c.$secondary-500;
            }
        }
    }

    figure::before{
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-image: linear-gradient(to right, c.$secondary-500 70%, c.$secondary-300);
        opacity: 0.3;
    }
            
    .card-col{
        gap: .5rem;
    }
</style>