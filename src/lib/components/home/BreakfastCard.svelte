<script>
	export let breakfast;
</script>

<div class="flex items-center justify-between border-b border-dashed border-gray-400 px-2 py-3">
	<div class="info flex items-center justify-center gap-4">
		<img src="/img/breakfast-1.jpg" alt="" class="w-20 rounded-full" />
		<!-- Name and contents -->
		<div>
			<h3 class="mb-2 text-xl font-light">{breakfast.name}</h3>
			<p class="text-base font-light text-gray-500">{breakfast.contents}</p>
		</div>
	</div>
	<p class="text-2xl font-light text-gray-700">${breakfast.price}</p>
</div>

<style></style>
