<script>

    let number = 10;
    let count = 0;

    function handleIncrement(event) {

        if(count < 10) {

            count += 1;

        } else {

            alert("Llegaste al máximo")

        }

    }

    function handleDecrement(event) {

        count -= 1;

        if (count < 0) {

            alert('No podes poner números negativos')
            count = 0;

        }

    }


</script>

{#if count == 10}
<p>Es igual a {count}</p>
{/if}

<h1>{count}</h1>

<button on:click={handleIncrement}>
    Incrementar
</button>

<button on:click={handleDecrement}>
    Decrementar
</button>


<style>
    
    h1 {

        color: cadetblue;

    }

</style>
