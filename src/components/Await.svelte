<script>
  let promise = new Promise((resolve, reject) => {
    setTimeout(() => {
      resolve("Datos recuperados");
    }, 2000);
  });
</script>

{#await promise}
  <!-- La promesa está pendiente -->
  <p>Esperando a que la promesa se resuelva...</p>
{:then value}
  <!-- La promesa se resolvió -->
  <p>El valor es {value}</p>
{:catch error}
  <!-- La promesa fue rechazada -->
  <p>Algo salió mal: {error.message}</p>
{/await}
