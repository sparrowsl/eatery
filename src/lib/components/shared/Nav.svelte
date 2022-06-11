<script>
	let hidden = true;
	function toggleMenu() {
		console.log('I have been clicked');
		hidden = !hidden;
	}
</script>

<section class="sticky top-0 bg-white">
	<nav
		class="container relative mx-auto flex min-h-[10vh] items-center justify-between lg:max-w-6xl"
	>
		<!-- Brand/Logo -->
		<div class="pl-3 text-2xl font-semibold italic">Eatery</div>

		<!-- Menu Items -->
		<div
			class:h-0={hidden}
			class:py-2={!hidden}
			class="items absolute top-full flex w-full flex-col gap-5 overflow-hidden
			bg-slate-50 px-4 shadow md:static md:h-fit md:w-fit md:flex-row md:bg-inherit md:p-0 md:shadow-none"
		>
			<a href="/" class="font-light">Home</a>
			<a href="/" class="font-light">About</a>
			<a href="/" class="font-light">Special Dishes</a>
			<a href="/" class="font-light">Menu</a>
			<a href="/" class="font-light">Team</a>
			<a href="/" class="font-light">Reservation</a>
		</div>

		<!-- Hamburger -->
		<div class="pr-3 text-2xl md:hidden" on:click={toggleMenu}>
			<i class="ri-menu-3-line" />
		</div>
	</nav>
</section>

<style></style>
