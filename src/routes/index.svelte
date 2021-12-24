<script context="module">
	export const prerender = true;
	import Carousel from '$lib/Carousel.svelte';

	const pc = [
		{ name: 'Gorrys-al-Lunn', path: 'pics/gorrys.jpeg' },
		{ name: 'Lysha-al-Rakath', path: 'pics/lysha.jpeg' },
		{ name: 'Ondren-al-Lemra', path: 'pics/ondren.jpeg' },
		{ name: 'Harlin-al-Kleve', path: 'pics/harlin.jpeg' },
		{ name: 'Kalas-al-Delsin', path: 'pics/kalas.jpeg' }
	];

	const litchton_manor = {
		label: 'Litchton Manor',
		items: [
			{ name: 'Sir Dalbar Vergent, Bailiff', path: 'pics/litchton/1/bailiff.jpeg' },
			{ name: 'Gandart Vergent, Chamberlain', path: 'pics/litchton/1/chamberlain.jpeg' },
			{ name: 'Bern, Man-at-arms', path: 'pics/litchton/1/man-at-arms-1.jpeg' },
			{ name: 'Trode, Man-at-arms', path: 'pics/litchton/1/man-at-arms-2.jpeg' },
			{ name: 'Denys, Man-at-arms', path: 'pics/litchton/1/man-at-arms-3.jpeg' },
			{ name: 'Niko-al-Trevor, Cook', path: 'pics/litchton/1/chef.jpeg' },
			{ name: 'Quilla-al-Lemra, Kitchen maid', path: 'pics/litchton/1/Quilla-al-Lemra.jpeg' },
			{ name: 'Shallya-al-Lemra, Chamber maid', path: 'pics/litchton/1/Shallya-al-Lemra.jpeg' },
			{ name: 'Tandar-al-Sendin, Stable Boy', path: 'pics/litchton/1/stable-boy.jpeg' }
		]
	};
</script>

<svelte:head>
	<title>The Gârgun Club</title>
</svelte:head>

<section>
	<div class="shadow card">
		<div class="card-body">
			<h1 class="card-title my-6 text-5xl font-bold md:place-self-center">
				<div class="avatar">
					<div class="mb-8 rounded-btn w-12 h-12">
						<img src="favicon.png" alt="a spiked club" />
					</div>
				</div>
				<span class="text-primary">Welome To The Gârgun Club</span>
				<div class="avatar">
					<div class="mb-8 rounded-btn w-12 h-12">
						<img src="favicon.png" alt="a spiked club" />
					</div>
				</div>
			</h1>
			<h3 class="text-3xl">Work in progress...</h3>
		</div>
	</div>
	<br />
	<p />
	<button class="btn btn-primary">Do Nothing</button>
	<button class="btn">Do As Little</button>

	<h2 class="text-2xl font-bold mb-1 mt-3">The adventurers in Asolade</h2>
	<Carousel items={pc} />

	<h2 class="text-2xl font-bold mb-1 mt-3">The people in Litchton, Daynora Hundred</h2>
	<Carousel label={litchton_manor.label} items={litchton_manor.items} />
</section>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@700&family=Lora&display=swap');

	section {
		font-family: 'Lora', serif;
	}
	h1,
	h2,
	h3 {
		font-family: 'Cinzel', serif;
	}
</style>
