<script lang="ts">
	import { getToastStore, type ToastSettings } from '@skeletonlabs/skeleton';

	const toastStore = getToastStore();

	const basicToast: ToastSettings = {
		message: 'Lorem ipsum dolor sit amet consectetur adipisicing elit...'
	};

	const actionToast: ToastSettings = {
		message: 'Lorem ipsum dolor sit amet consectetur adipisicing elit...',
		action: {
			label: 'Greeting',
			response: () => console.log('Hello, Skeleton')
		}
	};
</script>

<button class="btn variant-filled-primary" on:click={() => toastStore.trigger(basicToast)}
	>Basic Toast</button
>
<button class="btn variant-filled-primary" on:click={() => toastStore.trigger(actionToast)}
	>Action Toast</button
>

<button
	class="btn variant-filled-success"
	on:click={() => toastStore.trigger({ ...basicToast, background: 'variant-filled-success' })}
	>Success Toast</button
>
<button
	class="btn variant-filled-warning"
	on:click={() => toastStore.trigger({ ...basicToast, background: 'variant-filled-warning' })}
	>Warning Toast</button
>
<button
	class="btn variant-filled-error"
	on:click={() => toastStore.trigger({ ...basicToast, background: 'variant-filled-error' })}
	>Error Toast</button
>
