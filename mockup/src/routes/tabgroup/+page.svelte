<script lang="ts">
	import { Tabs } from '@skeletonlabs/skeleton-svelte';
</script>

<Tabs>
	{#snippet list()}
		<Tabs.Control value="tab1">Label 1</Tabs.Control>
		<Tabs.Control value="tab2">Label 2</Tabs.Control>
		<Tabs.Control value="tab3">Label 3</Tabs.Control>
	{/snippet}
	{#snippet content()}
		<Tabs.Panel value="tab1">(tab panel 1 contents)</Tabs.Panel>
		<Tabs.Panel value="tab2">(tab panel 2 contents)</Tabs.Panel><Tabs.Panel value="tab3">
			(tab panel 3 contents)
		</Tabs.Panel>
	{/snippet}
</Tabs>
