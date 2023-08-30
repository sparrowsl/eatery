<script>
	import { onNavigate } from '$app/navigation';
	import { formSuccess } from '$lib/store.js';
	import '../app.css';
	import Nav from '$lib/components/shared/Nav.svelte';
	import Footer from '$lib/components/shared/Footer.svelte';
	import OrderNotification from '$lib/components/OrderNotification.svelte';

	onNavigate(async (navigation) => {
		if (!document.startViewTransition) return;

		return new Promise((oldStateCaptureResolve) => {
			document.startViewTransition(async () => {
				oldStateCaptureResolve();
				await navigation.complete;
			});
		});
	});
</script>

{#if $formSuccess}
	<OrderNotification />
{/if}

<Nav />
<main>
	<slot />
</main>
<Footer />
