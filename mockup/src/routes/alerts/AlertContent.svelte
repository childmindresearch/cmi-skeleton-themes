<script lang="ts">
	import ThumbsUp from '$lib/ThumbsUp.svelte';

	export let text: string;
</script>

<div><ThumbsUp /></div>
<div class="alert-message">
	<h3 class="h3">(title)</h3>
	<p>{text}</p>
</div>
<div class="alert-actions"><button class="btn variant-filled">Button</button></div>
