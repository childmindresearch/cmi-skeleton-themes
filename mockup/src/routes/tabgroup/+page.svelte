<script lang="ts">
	import { Tab, TabGroup } from '@skeletonlabs/skeleton';

	let tabSet: number = 0;
</script>

<TabGroup>
	<Tab bind:group={tabSet} name="tab1" value={0}>
		<span>Label 1</span>
	</Tab>
	<Tab bind:group={tabSet} name="tab2" value={1}>Label 2</Tab>
	<Tab bind:group={tabSet} name="tab3" value={2}>Label 3</Tab>
	<svelte:fragment slot="panel">
		{#if tabSet === 0}
			(tab panel 1 contents)
		{:else if tabSet === 1}
			(tab panel 2 contents)
		{:else if tabSet === 2}
			(tab panel 3 contents)
		{/if}
	</svelte:fragment>
</TabGroup>
