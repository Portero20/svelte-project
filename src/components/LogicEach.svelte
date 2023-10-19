<script>
    let arrayItems = [
        { id: 1, name: "Item 1" },
        { id: 2, name: "Item 2" },
        { id: 3, name: "Item 3" },
    ];

</script>


<ul>
    {#each arrayItems as item (item.id)}
        <li class="item-{item.id}" id="item-{item.id}">{item.name}</li>
    {/each}
</ul>

<style>
    li {
        list-style-type: none;
    }
</style>
