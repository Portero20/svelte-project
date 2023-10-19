<script>
    const items = [
        {
            id: 1,
            title: "Titulo1",
        },
        {
            id: 2,
            title: "Titulo2",
        },
        {
            id: 3,
            title: "Titulo3",
        },
    ];
</script>

<ul>
    {#each items as item}
        <li class="fancy">
            <slot name="item" {item} />
        </li>
    {/each}
</ul>

<slot name="footer" />



