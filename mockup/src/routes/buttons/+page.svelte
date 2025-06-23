<script lang="ts">
	import ThumbsUp from '../../lib/ThumbsUp.svelte';
</script>

<!--Cannot loop due to CSS purging.-->
<div class="grid grid-cols-4 gap-2 mt-2 items-center align-middle">
	<button type="button" class="btn preset-filled-primary-500">Filled Primary</button>
	<button type="button" class="btn preset-filled-secondary-500">Filled Secondary</button>
	<button type="button" class="btn preset-filled-tertiary-500">Filled Tertiary</button>
	<button type="button" class="btn preset-filled-surface-500">Filled Surface</button>
	<button type="button" class="btn preset-tonal-primary">Tonal Primary</button>
	<button type="button" class="btn preset-tonal-secondary">Tonal Secondary</button>
	<button type="button" class="btn preset-tonal-tertiary">Tonal Tertiary</button>
	<button type="button" class="btn preset-tonal-surface">Tonal Surface</button>
	<button type="button" class="btn preset-outlined-primary-500">Outlined Primary</button>
	<button type="button" class="btn preset-outlined-secondary-500">Outlined Secondary</button>
	<button type="button" class="btn preset-outlined-tertiary-500">Outlined Tertiary</button>
	<button type="button" class="btn preset-outlined-surface-500">Outlined Surface</button>
	<button type="button" class="btn preset-filled-success-500">Filled Success</button>
	<button type="button" class="btn preset-filled-warning-500">Filled Warning</button>
	<button type="button" class="btn preset-filled-error-500">Filled Error</button>
</div>
