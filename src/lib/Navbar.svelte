<script>
    import ThemeButton from "./ThemeButton.svelte";
</script>

<div class="navbar mb-2 shadow ">
	<div class="flex-1 px-2 mx-2">
		<a href="/">
			<span class="text-lg font-bold">The Gârgun Club</span>
		</a>
	</div>
	<div class="flex-none">
		<a href="/" class="btn btn-ghost"> Home </a>
		<a href="/about" class="btn  btn-ghost"> About </a>
	</div>
    <ThemeButton/>
</div>