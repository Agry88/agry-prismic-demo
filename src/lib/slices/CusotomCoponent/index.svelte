<script>
	/** @type {import("@prismicio/client").Content.CusotomCoponentSlice} */
	export let slice;
</script>

<h1>{slice.primary.title}</h1>
<img class="img" src={slice.primary.image.url} alt={slice.primary.image.alt} />

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
