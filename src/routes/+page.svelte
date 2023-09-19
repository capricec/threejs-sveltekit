<script lang="ts">
	import { onMount } from 'svelte';
	import { createScene } from '$lib/scene';

	let el:HTMLCanvasElement;

	onMount(() => {
		createScene(el);
	});
</script>

<svelte:head>
	<title>Fanout FanPulse</title>
	<meta name="description" content="Fanout Fan Pulse Visualization" />
</svelte:head>

<canvas bind:this={el} />
