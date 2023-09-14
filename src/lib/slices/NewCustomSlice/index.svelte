<script>
	/** @type {import("@prismicio/client").Content.NewCustomSliceSlice} */
	export let slice;
</script>

{#if slice.variation === 'default'}
	<div>
		<h1>{slice.primary.text}</h1>
		<img class="img" src={slice.primary.image.url} alt={slice.primary.image.alt} />
		<ul>
			{#each slice.items as item}
				<li>{item.selectlabel}</li>
			{/each}
		</ul>
	</div>
{/if}

<style lang="scss">
	.img {
		width: 100px;
		height: 100px;

		&:hover {
			width: 200px;
			height: 200px;
		}
	}
</style>
