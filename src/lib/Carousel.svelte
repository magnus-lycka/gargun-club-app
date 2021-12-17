<script>
	import CarouselItem from "./CarouselItem.svelte";

	export let label = null;
	export let items = [];
</script>

<div>
	{#if label}
	<h3 class="text-xl font-bold mb-1 mt-1">{label}</h3>	
	{/if}

	<div class="my-2 p-4 space-x-4 carousel carousel-center bg-neutral rounded-box">
		{#each items as {name, path}}
		<CarouselItem {name} {path}/>
		{/each}
	</div>
</div>

