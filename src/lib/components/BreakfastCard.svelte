<script>
	export let breakfast;
</script>

<div class="flex items-center justify-between border-b border-dashed border-gray-400 px-2 py-3">
	<figure class="info flex items-center justify-center gap-4">
		<img src="/img/{breakfast?.image ?? 'breakfast-1.jpg'}" alt="" class="w-20 rounded-full" />
		<!-- Name and contents -->
		<figcaption>
			<h3 class="mb-2 text-xl font-light">{breakfast.name}</h3>
			<p class="text-base font-light text-gray-500">{breakfast.contents}</p>
		</figcaption>
	</figure>
	<p class="text-2xl font-light text-gray-700">${breakfast.price}</p>
</div>
