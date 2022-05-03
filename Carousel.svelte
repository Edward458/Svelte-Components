<script>
	// Simple carousel
	// May or may not need an image item, using gallery items could work
	export let numImages;
	export let slideDuration = 4000;
	export let carouselImages;
	$: active = carouselImages[0].description;
	setInterval(() => {
		if (active > numImages) active = 0;
		else active++;
	}, slideDuration);
</script>

<div class="carousel">
	{#each carouselImages as image}
		<div
			class={active == image.description
				? "carousel-item active"
				: "carousel-item"}
		>
			<img src={image.link} alt={image.name} />
		</div>
	{/each}
</div>

<style>
	.carousel{
		margin:0;
		padding: 0;
	}
	.carousel-item {
		display: none;
		margin:0;
		padding: 0;
	
	}

	.active {
		display: block;
	}


</style>
