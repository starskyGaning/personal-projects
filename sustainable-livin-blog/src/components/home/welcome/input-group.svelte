<script>
    export let subscriptionButtonName = "Subscribe Now";
</script>

<div class="input-group">
    <input type="email" class="form-control" placeholder="Your Email Here" aria-label="email-input" aria-describedby="email-button">
    <button class="btn" type="button" id="email-button">{subscriptionButtonName}</button>
</div>

<style lang="scss">
    @use '../../../resources/scss/compiler' as c;

    .input-group{
        input{
            @include c.body;
            border: 4px c.$secondary-500 solid;
            border-radius: 0;
        }
        button{
            @include c.heading-3;
            background-color: c.$secondary-500;
            border-radius: 0;
            color: c.$primary-500;
            padding: 1rem 1.5rem;
            transition: all 800ms ease;
        }
        button:hover{
            background-color: c.$primary-500;
            color: c.$secondary-500;
        }
    }
</style>