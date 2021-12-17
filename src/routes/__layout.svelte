<script>
	import Footer from '$lib/Footer.svelte';
	import Navbar from '$lib/Navbar.svelte';
	import '../app.css';
</script>

<div>
	<Navbar />
	<main>
		<slot />
	</main>

	<Footer />
</div>