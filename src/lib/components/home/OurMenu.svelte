<script>
	import BreakfastCard from './BreakfastCard.svelte';

	const breakfasts = [
		{
			name: 'Egg Sandwich',
			contents: 'Meat Ball, Mie',
			price: 30
		},
		{
			name: 'Egg Sandwich',
			contents: 'Meat Ball, Mie',
			price: 30
		},
		{
			name: 'Egg Sandwich',
			contents: 'Meat Ball, Mie',
			price: 30
		},
		{
			name: 'Egg Sandwich',
			contents: 'Meat Ball, Mie',
			price: 30
		},
		{
			name: 'Egg Sandwich',
			contents: 'Meat Ball, Mie',
			price: 30
		},
		{
			name: 'Egg Sandwich',
			contents: 'Meat Ball, Mie',
			price: 30
		},
		{
			name: 'Egg Sandwich',
			contents: 'Meat Ball, Mie',
			price: 30
		},
		{
			name: 'Egg Sandwich',
			contents: 'Meat Ball, Mie',
			price: 30
		},
		{
			name: 'Egg Sandwich',
			contents: 'Meat Ball, Mie',
			price: 30
		}
	];
</script>

<section class="container mx-auto min-h-screen py-16 px-2 lg:max-w-6xl">
	<!-- Banner -->
	<div class="mb-12 text-center">
		<p class="text-base text-red-400">Specialities</p>
		<h2 class="text-2xl font-bold">Our Menu</h2>
	</div>

	<section class="menu grid lg:grid-cols-3 lg:gap-10">
		{#each breakfasts as breakfast}
			<BreakfastCard {breakfast} />
		{/each}
	</section>
</section>

<style></style>
