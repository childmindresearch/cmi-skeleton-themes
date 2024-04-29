<script lang="ts">
	import ThumbsUp from '../../lib/ThumbsUp.svelte';
</script>

<button type="button" class="btn-icon variant-soft-primary"><ThumbsUp /></button>
<button type="button" class="btn variant-soft-primary">Button</button>
<button type="button" class="btn variant-soft-primary">
	<span><ThumbsUp /></span>
	<span>Button</span>
</button>

<div class="btn-group variant-soft-primary">
	<button>Months</button>
	<button>Days</button>
	<button>Years</button>
</div>

<!--Cannot loop due to CSS purging.-->
<div class="grid grid-cols-4 gap-2 mt-2 items-center align-middle">
	<button type="button" class="btn variant-soft-primary">soft primary</button>
	<button type="button" class="btn variant-ghost-primary">ghost primary</button>
	<button type="button" class="btn variant-outline-primary">outline primary</button>
	<button type="button" class="btn variant-filled-primary">filled primary</button>
	<button type="button" class="btn variant-soft-secondary">soft secondary</button>
	<button type="button" class="btn variant-ghost-secondary">ghost secondary</button>
	<button type="button" class="btn variant-outline-secondary">outline secondary</button>
	<button type="button" class="btn variant-filled-secondary">filled secondary</button>
	<button type="button" class="btn variant-soft-tertiary">soft tertiary</button>
	<button type="button" class="btn variant-ghost-tertiary">ghost tertiary</button>
	<button type="button" class="btn variant-outline-tertiary">outline tertiary</button>
	<button type="button" class="btn variant-filled-tertiary">filled tertiary</button>
	<button type="button" class="btn variant-soft-success">soft success</button>
	<button type="button" class="btn variant-ghost-success">ghost success</button>
	<button type="button" class="btn variant-outline-success">outline success</button>
	<button type="button" class="btn variant-filled-success">filled success</button>
	<button type="button" class="btn variant-soft-warning">soft warning</button>
	<button type="button" class="btn variant-ghost-warning">ghost warning</button>
	<button type="button" class="btn variant-outline-warning">outline warning</button>
	<button type="button" class="btn variant-filled-warning">filled warning</button>
	<button type="button" class="btn variant-soft-error">soft error</button>
	<button type="button" class="btn variant-ghost-error">ghost error</button>
	<button type="button" class="btn variant-outline-error">outline error</button>
	<button type="button" class="btn variant-filled-error">filled error</button>
	<button type="button" class="btn variant-soft-surface">soft surface</button>
	<button type="button" class="btn variant-ghost-surface">ghost surface</button>
	<button type="button" class="btn variant-outline-surface">outline surface</button>
	<button type="button" class="btn variant-filled-surface">filled surface</button>
</div>
