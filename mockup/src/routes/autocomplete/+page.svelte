<script lang="ts">
	import { Combobox } from '@skeletonlabs/skeleton-svelte';

	interface ComboboxData {
		label: string;
		value: string;
	}

	let selectedFlavor: string[] = $state([]);

	const comboboxData: ComboboxData[] = [
		{ label: 'Vanilla', value: 'vanilla' },
		{ label: 'Chocolate', value: 'chocolate' },
		{ label: 'Strawberry', value: 'strawberry' },
		{ label: 'Pineapple', value: 'pineapple' },
		{ label: 'Peach', value: 'peach' }
	];
</script>

<Combobox
	data={comboboxData}
	value={selectedFlavor}
	onValueChange={(e) => (selectedFlavor = e.value)}
	label="Select Flavor"
	placeholder="Select..."
></Combobox>
