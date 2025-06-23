<script lang="ts">
	import NavBar from '$lib/components/NavBar.svelte';
	import Navigation from '$lib/components/Navigation.svelte';
	import { Toaster } from '@skeletonlabs/skeleton-svelte';
	import { toaster } from '$lib/toast';
	import '../app.css';

	let { children } = $props();
</script>

<svelte:head>
	<title>Skeleton Theme Mock-Up</title>
</svelte:head>

<Toaster {toaster}></Toaster>
<header><NavBar /></header>

<div class="flex h-screen">
	<div class="hidden md:block md:w-64 h-full z-10 flex-shrink-0">
		<Navigation />
	</div>

	<div class="overflow-y-hidden px-10 pt-5 flex-1">
		{@render children()}
	</div>
</div>
