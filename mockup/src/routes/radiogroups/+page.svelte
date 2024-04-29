<script lang="ts">
	import { RadioGroup, RadioItem } from '@skeletonlabs/skeleton';

	let value1: number = 0;
	let value2: number = 0;
</script>

<RadioGroup>
	<RadioItem bind:group={value1} name="justify" value={0}>Label 0</RadioItem>
	<RadioItem bind:group={value1} name="justify" value={1}>Label 1</RadioItem>
	<RadioItem bind:group={value1} name="justify" value={2}>Label 2</RadioItem>
</RadioGroup>

<RadioGroup flexDirection="flex-col">
	<RadioItem bind:group={value2} name="justify" value={0}>Label 0</RadioItem>
	<RadioItem bind:group={value2} name="justify" value={1}>Label 1</RadioItem>
	<RadioItem bind:group={value2} name="justify" value={2}>Label 2</RadioItem>
</RadioGroup>
