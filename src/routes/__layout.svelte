<script>
	import Footer from '$lib/Footer.svelte';
	import Navbar from '$lib/Navbar.svelte';
	import '../app.css';
</script>

<div class="flex flex-col min-h-screen">
	<Navbar />
	<main class="flex-grow">
		<slot />
	</main>

	<Footer />
</div>