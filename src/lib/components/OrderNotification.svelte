<script>
	import 'iconify-icon';
	import { fly } from 'svelte/transition';
	import { formSuccess } from '$lib/store.js';
</script>

<div
	transition:fly={{ y: -200, duration: 500 }}
	class="fixed top-0 z-40 flex w-full items-center justify-between rounded bg-green-200 p-4 shadow-md"
>
	<p>Your order was successful!! Thanks for coming.</p>
	<button class="text-2xl text-green-600" on:click={() => ($formSuccess = false)}>
		<iconify-icon icon="carbon:close" />
	</button>
</div>
