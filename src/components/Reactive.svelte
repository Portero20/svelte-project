<script>
    export let saludo = "Mundo";
    // Valor inicial
    let length = saludo.length;
    // Cambio reactivo, solo cuando se modifica saludo
    $: length = saludo.length;
</script>

<input type="text" bind:value={saludo} />
<span>{length}</span>
<h1>
    Hola {saludo}
</h1>

<style>
    h1 {
        color: tomato;
    }
</style>
