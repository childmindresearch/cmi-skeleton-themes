<script lang="ts">
	import { AppBar } from '@skeletonlabs/skeleton-svelte';
	import { Modal } from '@skeletonlabs/skeleton-svelte';

	let drawerState = $state(false);
</script>

<AppBar background="bg-surface-50">
	{#snippet trail()}
		<button class="btn hover:variant-soft-primary">
			<a
				data-testid="a-github"
				href="https://github.com/childmindresearch/cmi-skeleton-themes"
				target="_blank"
				rel="noreferrer"
			>
				<i class="fa-brands fa-github text-lg"></i>
				<span>GitHub</span>
			</a>
		</button>
		<button class="btn hover:variant-soft-primary">
			<a data-testid="a-mailto" href="mailto:dair@childmind.org" target="_blank" rel="noreferrer">
				<i class="fa-solid fa-envelope text-lg"></i>
				<span>Contact</span>
			</a>
		</button>
	{/snippet}
</AppBar>
