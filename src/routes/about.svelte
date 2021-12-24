<script context="module">
	import { browser, dev } from '$app/env';

	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	export const hydrate = dev;

	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	export const router = browser;

	// since there's no dynamic data here, we can prerender
	// it so that it gets served as a static asset in prod
	export const prerender = true;
</script>

<svelte:head>
	<title>About Gârgun Club</title>
</svelte:head>

<div class="content">
	<div class="flex-1 px-8 mx-8">
		<h1 class="text-3xl font-bold mb-1 mt-3">About the Gârgun Club</h1>

		<p>
			This site is intended to provide support for my (Magnus Lyckå) role-playing activities, and
			for the people I play with, but parts of it will hopefully be useful for more people
			interested in role-playing etc.
		</p>

		<h2 class="text-2xl font-bold mb-1 mt-3">Contributing</h2>

		<p>TBD...</p>
	</div>
</div>

<style>
	.content {
		width: 100%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}
</style>
