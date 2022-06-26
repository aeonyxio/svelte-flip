<script lang="ts">
	import Flippable from '$lib/Flippable.svelte';
	let flip = false;
</script>

<button on:click={() => (flip = !flip)}>Flip!</button>
<main>
	<Flippable height="337px" width="234px" {flip}>
		<img slot="front" src="/card-front.png" />
		<img slot="back" src="/card-back.png" />
	</Flippable>
</main>

<style>
	img {
		box-shadow: 0px 3px 18px 3px rgba(0, 0, 0, 0.2);
	}
</style>
