<script>
    export let bootIconName;
    export let socialDist = '/';
</script>


<a href="{socialDist}"><i class="bi {bootIconName}"></i></a>

<style lang="scss">
    @use '../../resources/scss/compiler' as c;

    a{
        transition: all 800ms ease;
        i{
            color: c.$primary-500;
            font-size: 2rem;
            transition: all 800ms ease;
        }
    }
    a:hover{
        transform: scale(1.5);
        margin: 0 .5rem;
        i{
            color: c.$secondary-400;
        }
    }
    
</style>