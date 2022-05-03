<script context="module" lang="ts">
	export const prerender = true;
</script>

<svelte:head>
	<title>ProTrailblazer.com</title>
	<meta name="description" content="ProTrailblazer.com" />
</svelte:head>

<section>
	<div class="youtube">
		<a href="https://www.youtube.com/channel/UCw_DRwblLZd7OF38mc9qFeg">
			<picture>
				<source srcset="youtube.svg" type="image/svg" />
				<img src="youtube.svg" alt="youtube" />
			</picture>
		</a>
	</div>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	.youtube {
		position: relative;
		margin: 0 auto;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}
</style>
