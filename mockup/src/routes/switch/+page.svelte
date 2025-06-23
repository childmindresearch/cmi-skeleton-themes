<script lang="ts">
	import { Switch } from '@skeletonlabs/skeleton-svelte';

	let checked = $state(false);
</script>

<Switch name="slider-label" onCheckedChange={(e) => (checked = e.checked)}>Switch</Switch>
