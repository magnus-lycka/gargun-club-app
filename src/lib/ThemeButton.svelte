<script>
	import { onMount } from 'svelte';

	const darkTheme = 'luxury';
	const lightTheme = 'garden';

	onMount(() => {
		if (!document.documentElement.getAttribute('data-theme')) {
			document.documentElement.setAttribute('data-theme', lightTheme);
		}
	});

	function nextTheme() {
		if (document.documentElement.getAttribute('data-theme') != lightTheme) {
			console.log('Go light');
			document.documentElement.setAttribute('data-theme', lightTheme);
		} else {
			document.documentElement.setAttribute('data-theme', darkTheme);
			console.log('Go dark');
		}
	}
</script>

<button class="btn btn-accent" on:click={nextTheme}> Light/Dark </button>
