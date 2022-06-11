<script>
	import '../tailwind.css';
	import 'remixicon/fonts/remixicon.css';
	import Nav from '$lib/components/shared/Nav.svelte';
	import Footer from '$lib/components/Footer.svelte';
</script>

<Nav />
<main class="px-2">
	<slot />
</main>
<Footer />

<style></style>
