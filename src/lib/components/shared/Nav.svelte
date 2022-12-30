<script>
	import 'iconify-icon';
	import { beforeNavigate } from '$app/navigation';

	beforeNavigate(() => (isOpen = false));

	let isOpen = false;
</script>

<section class="sticky top-0 bg-white lg:static">
	<nav class="container relative mx-auto flex min-h-[10vh] max-w-6xl items-center justify-between">
		<!-- Brand/Logo -->
		<a href="/" class="pl-3 text-2xl font-semibold italic md:p-0">Eatery</a>

		<!-- Menu Items -->
		<div
			class="{isOpen
				? 'py-2'
				: 'h-0'} items absolute top-full flex w-full flex-col gap-5 overflow-hidden
			bg-slate-50 px-4 shadow md:static md:h-fit md:w-fit md:flex-row md:bg-inherit md:p-0 md:shadow-none"
		>
			<a href="/" class="font-light">Home</a>
			<a href="/about" class="font-light">About</a>
			<a href="/special" class="font-light">Special Dishes</a>
			<a href="/menu" class="font-light">Menu</a>
			<a href="/team" class="font-light">Team</a>
			<a href="/reservation" class="font-light">Reservation</a>
		</div>

		<!-- Hamburger -->
		<!-- svelte-ignore a11y-click-events-have-key-events -->
		<span class="pr-3 text-2xl md:hidden" on:click={() => (isOpen = !isOpen)}>
			<iconify-icon icon="material-symbols:menu-open" />
		</span>
	</nav>
</section>

<style></style>
