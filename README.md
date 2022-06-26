# svelte-flip

A simple, light-weight, flippable card component written with SvelteKit. The source code and an example can be found in [this blog post](https://aeonyx.io/code/blog/svelte-flippable-card-component).

## Install

```bash
npm i svelte-flip
```

## Usage

```svelte
<script lang="ts">
	import { Flippable } from 'svelte-flip';
	let flip = false;
</script>

<button on:click={() => (flip = !flip)}>Flip!</button>
<Flippable height="337px" width="234px" {flip}>
	<img slot="front" src="/card-front.png" />
	<img slot="back" src="/card-back.png" />
</Flippable>
```
