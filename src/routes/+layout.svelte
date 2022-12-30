<script>
	import { formSuccess } from '$lib/store.js';
	import '../app.css';
	import Nav from '$lib/components/shared/Nav.svelte';
	import Footer from '$lib/components/shared/Footer.svelte';
	import OrderNotification from '$lib/components/OrderNotification.svelte';
</script>

{#if $formSuccess}
	<OrderNotification />
{/if}

<Nav />
<main>
	<slot />
</main>
<Footer />
