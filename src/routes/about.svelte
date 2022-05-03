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
	<title>About ProTrailblazer.com</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="content">
	<h1>About ProTrailblazer.com</h1>

	<p>
		My name is Ryan Murray and I am a freelance digital creative of 20+ years. My work is in a
		variety of forms. These include:
	</p>

	<ul>
		<li>Fullstack Web Development</li>
		<li>SEO Strategy</li>
		<li>Product Photography</li>
		<li>Motion Graphics</li>
		<li>Game Development</li>
		<li>Music Production</li>
		<li>Video Post Production</li>
		<li>Digital Illustration</li>
	</ul>

	<p>
		Currently 100% of my offerings will be published on youtube: <a
			href="https://www.youtube.com/channel/UCw_DRwblLZd7OF38mc9qFeg/videos">Subscribe Here</a
		>
	</p>
</div>

<style>
	.content {
		width: 100%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}
</style>
