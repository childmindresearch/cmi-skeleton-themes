<script lang="ts">
	import { Navigation } from '@skeletonlabs/skeleton-svelte';
	import { page } from '$app/state';

	let isExpanded = $state(true);

	const pages = [
		{ name: 'Autocomplete', href: '/autocomplete' },
		{ name: 'Buttons', href: '/buttons' },
		{ name: 'Hr', href: '/hr' },
		{ name: 'Input', href: '/input' },
		{ name: 'Segment', href: '/segment' },
		{ name: 'Switch', href: '/switch' },
		{ name: 'Tab Group', href: '/tabgroup' },
		{ name: 'Table', href: '/table' },
		{ name: 'Toasts', href: '/toasts' },
		{ name: 'Typography', href: '/typography' }
	];
</script>

<div
	class="bg-surface-50 border-surface-50 grid h-full w-full grid-cols-[auto_1fr] border-[1px] card"
>
	<Navigation.Rail expanded={isExpanded} background="bg-surface-50" tilesJustify="justify-start">
		{#snippet tiles()}
			{#each pages as { name, href }}
				<Navigation.Tile {href} selected={page.url.pathname === href}>
					{name}
				</Navigation.Tile>
			{/each}
		{/snippet}
	</Navigation.Rail>
</div>
