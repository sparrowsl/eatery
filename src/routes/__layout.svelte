<script>
	import { fly } from 'svelte/transition';
	import { formSuccess } from '../lib/store';
	import '../tailwind.css';
	import 'remixicon/fonts/remixicon.css';
	import Nav from '$lib/components/shared/Nav.svelte';
	import Footer from '$lib/components/shared/Footer.svelte';
</script>

{#if $formSuccess}
	<div
		class="fixed top-0 min-h-[5vh] w-full bg-green-200 p-5 text-green-700"
		transition:fly={{ y: -200, duration: 750 }}
	>
		You order has been submitted successfully!! Thanks for coming.
	</div>
{/if}

<Nav />
<main>
	<slot />
</main>
<Footer />

<style></style>
