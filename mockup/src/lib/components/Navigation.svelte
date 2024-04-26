<script lang="ts">
	import { page } from '$app/stores';
	import { getDrawerStore } from '@skeletonlabs/skeleton';

	const drawerStore = getDrawerStore();
	const pages = [
		{ name: 'Buttons', href: '/buttons' },
		{ name: 'Slide Toggle', href: '/slidetoggle' },
		{ name: 'Table', href: '/table' }
	];

	function drawerClose(): void {
		drawerStore.close();
	}

	$: classesActive = (href: string) =>
		href === $page.url.pathname ? 'bg-primary-100 dark:bg-primary-700' : '';
</script>

<nav class="list-nav p-4 flex flex-col" data-testid="div-navigation">
	<ul style="flex-grow: 1;">
		{#each pages as { name, href }}
			<li>
				<a {href} class={classesActive(href)} data-testid="a-navigation" on:click={drawerClose}
					>{name}</a
				>
			</li>
		{/each}
	</ul>
</nav>
