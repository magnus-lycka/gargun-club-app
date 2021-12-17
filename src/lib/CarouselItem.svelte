<script>
	export let name;
	export let path;
</script>

<div data-tip={name} class="carousel-item tooltip tooltip-open tooltip-bottom mb-6">
	<img height="200" width="200" src={path} alt="picture of {name}" />
</div>
