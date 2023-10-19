<script>
    let name = "world";
    // a los 2 segundos, queremos que name pase a ser "frontender"
    setTimeout(function () {
        name = "frontender";
    }, 2000);
</script>

<h1>Hello {name}!</h1>

<style>
    h1 {
        font-weight: 100;
        text-transform: uppercase;
    }
</style>
