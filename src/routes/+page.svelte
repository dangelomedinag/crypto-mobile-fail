<script>
	let arr = [];
	const add = () => (arr = [{ id: crypto.randomUUID() }, ...arr]);
</script>

<button on:click={add}>add</button>
{#each arr as item (item.id)}
	<p>{item.id}</p>
{/each}
