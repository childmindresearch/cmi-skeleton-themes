<script lang="ts">
	import AlertContent from './AlertContent.svelte';
</script>

<!-- Variants written out in full due to CSS purge.-->
<div class="grid grid-cols-2 gap-2">
	<aside class="alert variant-ghost"><AlertContent text="variant ghost" /></aside>
	<aside class="alert variant-ghost-surface"><AlertContent text="variant ghost surface" /></aside>
	<aside class="alert variant-ghost-primary"><AlertContent text="variant ghost primary" /></aside>
	<aside class="alert variant-ghost-secondary">
		<AlertContent text="variant ghost secondary" />
	</aside>
	<aside class="alert variant-ghost-tertiary"><AlertContent text="variant ghost tertiary" /></aside>
	<aside class="alert variant-ghost-success"><AlertContent text="variant ghost success" /></aside>
	<aside class="alert variant-ghost-warning"><AlertContent text="variant ghost warning" /></aside>
	<aside class="alert variant-ghost-error"><AlertContent text="variant ghost error" /></aside>

	<aside class="alert variant-filled"><AlertContent text="variant filled" /></aside>
	<aside class="alert variant-filled-surface"><AlertContent text="variant filled surface" /></aside>
	<aside class="alert variant-filled-primary"><AlertContent text="variant filled primary" /></aside>
	<aside class="alert variant-filled-secondary">
		<AlertContent text="variant filled secondary" />
	</aside>
	<aside class="alert variant-filled-tertiary">
		<AlertContent text="variant filled tertiary" />
	</aside>
	<aside class="alert variant-filled-success"><AlertContent text="variant filled success" /></aside>
	<aside class="alert variant-filled-warning"><AlertContent text="variant filled warning" /></aside>
	<aside class="alert variant-filled-error"><AlertContent text="variant filled error" /></aside>

	<aside class="alert variant-ringed"><AlertContent text="variant ringed" /></aside>
	<aside class="alert variant-ringed-surface"><AlertContent text="variant ringed surface" /></aside>
	<aside class="alert variant-ringed-primary"><AlertContent text="variant ringed primary" /></aside>
	<aside class="alert variant-ringed-secondary">
		<AlertContent text="variant ringed secondary" />
	</aside>
	<aside class="alert variant-ringed-tertiary">
		<AlertContent text="variant ringed tertiary" />
	</aside>
	<aside class="alert variant-ringed-success"><AlertContent text="variant ringed success" /></aside>
	<aside class="alert variant-ringed-warning"><AlertContent text="variant ringed warning" /></aside>
	<aside class="alert variant-ringed-error"><AlertContent text="variant ringed error" /></aside>

	<aside class="alert variant-soft"><AlertContent text="variant soft" /></aside>
	<aside class="alert variant-soft-surface"><AlertContent text="variant soft surface" /></aside>
	<aside class="alert variant-soft-primary"><AlertContent text="variant soft primary" /></aside>
	<aside class="alert variant-soft-secondary"><AlertContent text="variant soft secondary" /></aside>
	<aside class="alert variant-soft-tertiary"><AlertContent text="variant soft tertiary" /></aside>
	<aside class="alert variant-soft-success"><AlertContent text="variant soft success" /></aside>
	<aside class="alert variant-soft-warning"><AlertContent text="variant soft warning" /></aside>
	<aside class="alert variant-soft-error"><AlertContent text="variant soft error" /></aside>

	<aside class="alert bg-gradient-to-br variant-gradient-primary-secondary">
		<AlertContent text="variant gradient primary secondary" />
	</aside>
	<aside class="alert bg-gradient-to-br variant-gradient-secondary-primary">
		<AlertContent text="variant gradient secondary primary" />
	</aside>
	<aside class="alert bg-gradient-to-br variant-gradient-primary-tertiary">
		<AlertContent text="variant gradient primary tertiary" />
	</aside>
</div>
