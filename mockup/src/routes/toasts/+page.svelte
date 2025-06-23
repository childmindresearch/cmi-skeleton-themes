<script lang="ts">
	import { toaster } from '$lib/toast';

	const toastMessage = { title: 'Title', description: 'This is a description.' };
</script>

<button class="btn preset-filled-primary-500" on:click={() => toaster.info(toastMessage)}
	>Info Toast</button
>
<button class="btn preset-filled-success-500" on:click={() => toaster.success(toastMessage)}
	>Success Toast</button
>
<button class="btn preset-filled-warning-500" on:click={() => toaster.warning(toastMessage)}
	>Warning Toast</button
>
<button class="btn preset-filled-error-500" on:click={() => toaster.error(toastMessage)}
	>Error Toast</button
>
