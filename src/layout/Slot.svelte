<div>
	<slot name="title" />
	{#if $$slots.description}
		<!-- This <hr> and slot will render only if a slot named "description" is provided. -->
		<hr />
		<slot name="description" />
	{/if}
</div>