<script>
	import 'iconify-icon';

	const staff = [
		{
			name: 'Aaron Patel',
			position: 'CEO',
			image: 'chef-1.jpg',
			socials: [
				{ icon: 'mdi:twitter', url: '' },
				{ icon: 'mdi:facebook', url: '' },
				{ icon: 'material-symbols:mail', url: '' },
				{ icon: 'mdi:instagram', url: '' }
			]
		},
		{
			name: 'Daniel Tebas',
			position: 'Chef',
			image: 'chef-2.jpg',
			socials: [
				{ icon: 'mdi:twitter', url: '' },
				{ icon: 'mdi:facebook', url: '' },
				{ icon: 'material-symbols:mail', url: '' },
				{ icon: 'mdi:instagram', url: '' }
			]
		},
		{
			name: 'John Snow',
			position: 'Chef',
			image: 'chef-3.jpg',
			socials: [
				{ icon: 'mdi:twitter', url: '' },
				{ icon: 'mdi:facebook', url: '' },
				{ icon: 'material-symbols:mail', url: '' },
				{ icon: 'mdi:instagram', url: '' }
			]
		}
	];
</script>

<article class="container mx-auto min-h-[90vh] py-16 lg:max-w-6xl">
	<div class="mb-12 text-center">
		<p class="text-base text-red-400">Specialities</p>
		<h1 class="text-2xl font-bold">Our Team</h1>
	</div>

	<!-- Team members -->
	<section class="grid gap-10 md:grid-cols-3 md:gap-5 lg:px-10">
		{#each staff as user (user)}
			<figure class="px-4">
				<img src="/img/{user.image}" alt="" class="" />
				<figcaption class="text-center">
					<h3 class="font-josefin mt-1 text-2xl font-normal">{user.name}</h3>
					<p class="font-light">{user.position}</p>
					<!-- Social contacts -->
					<div class="mt-2 flex justify-center gap-5 text-xl text-red-500">
						{#each user.socials as social}
							<a href={social.url}><iconify-icon icon={social.icon} /></a>
						{/each}
					</div>
				</figcaption>
			</figure>
		{/each}
	</section>
</article>
