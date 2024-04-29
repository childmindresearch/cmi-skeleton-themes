<script lang="ts">
	import NavBar from '$lib/components/NavBar.svelte';
	import Navigation from '$lib/components/Navigation.svelte';
	import '@cmi-dair/skeleton-themes/cmi.postcss';
	import { arrow, autoUpdate, computePosition, flip, offset, shift } from '@floating-ui/dom';
	import {
		AppShell,
		Drawer,
		Toast,
		initializeStores,
		storeHighlightJs,
		storePopup
	} from '@skeletonlabs/skeleton';
	import hljs from 'highlight.js/lib/core';
	import css from 'highlight.js/lib/languages/css';
	import javascript from 'highlight.js/lib/languages/javascript';
	import typescript from 'highlight.js/lib/languages/typescript';
	import xml from 'highlight.js/lib/languages/xml';
	import 'highlight.js/styles/github-dark.css';
	import '../app.postcss';

	hljs.registerLanguage('xml', xml); // for HTML
	hljs.registerLanguage('css', css);
	hljs.registerLanguage('javascript', javascript);
	hljs.registerLanguage('typescript', typescript);
	storeHighlightJs.set(hljs);

	// Floating UI for Popups
	storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });

	initializeStores();
</script>

<svelte:head>
	<title>Skeleton Theme Mock-Up</title>
</svelte:head>

<Toast />
<Drawer width="w-64">
	<h2 class="p-4 h2">Navigation</h2>
	<hr />
	<Navigation />
</Drawer>

<AppShell slotSidebarLeft="bg-surface-500/5 w-0 md:w-64">
	<svelte:fragment slot="header">
		<NavBar />
	</svelte:fragment>
	<svelte:fragment slot="sidebarLeft">
		<Navigation />
	</svelte:fragment>
	<div class="max-w-screen-md mx-auto mt-5 px-5 min-w-[332px]">
		<slot />
	</div>
</AppShell>
