<script>
    let count = 3;
</script>

<div>
    {#if count > 0}
        <p>Contando... {count}</p>
        <svelte:self count={count - 1} />
    {:else}
        <p>¡Despegue!</p>
    {/if}
</div>

