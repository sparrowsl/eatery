<script>
	import 'iconify-icon';
</script>

<header class="container mx-auto flex max-w-6xl flex-col justify-center px-2 md:min-h-screen">
	<h1 class="font-josefin my-10 text-6xl font-light md:max-w-[12ch]">We Love Delicious Foods!</h1>

	<!-- Call to actions -->
	<div class="mb-10">
		<a
			href="/menu"
			class="block w-fit rounded-full bg-red-500 py-2 px-5 font-semibold text-white shadow
				shadow-red-200 hover:bg-red-600"
		>
			Explore Menu
		</a>
	</div>

	<!-- Extra features -->
	<ul class="font-josefin flex gap-5">
		<li class="flex flex-col items-center text-2xl">
			<iconify-icon icon="bi:rocket-takeoff" class="mb-2 text-4xl" />
			<span class="font-normal">Fast delivery</span>
		</li>
		<li class="flex flex-col items-center text-2xl">
			<iconify-icon icon="ion:leaf-outline" class="mb-2 text-4xl" />
			<span class="font-normal">Fresh Food</span>
		</li>
		<li class="flex flex-col items-center text-2xl">
			<iconify-icon icon="mdi:chat-outline" class="mb-2 text-4xl" />
			<span class="font-normal">24/7 Support</span>
		</li>
	</ul>

	<!-- Display some foods -->
	<div class="mt-10 grid grid-cols-3 gap-1 md:gap-5 lg:gap-0">
		<img src="/img/hero-1.jpg" alt="" class="lg:w-3/4" />
		<img src="/img/hero-2.jpg" alt="" class="lg:w-3/4" />
		<img src="/img/hero-3.jpg" alt="" class="lg:w-3/4" />
	</div>
</header>
