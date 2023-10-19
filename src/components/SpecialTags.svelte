<script>

let post = {
    id: 1,
    title: "Este es un post",
    content: "<p>Este es el contenido <strong>HTML</strong> de la publicación.</p>"
};

let user = {

    firstName: 'Exequiel',
    lastName: 'Portero'
}

export let boxes = [

    { width: 10, height: 5 },
    { width: 8, height: 3 },
    { width: 12, height: 6 }

];

</script>

<div>
    <h1>{post.title}</h1>
    {@html post.content} 
    {@html "<div>"}content{@html "</div>"}
</div>

<div>

    {@debug user}

    <h1>Hello {user.firstName}</h1>

</div>

{#each boxes as box}
  {@const area = box.width * box.height}
  <p>{box.width} * {box.height} = {area}</p>
{/each}


