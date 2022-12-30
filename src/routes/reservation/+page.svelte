<script>
	import { enhance } from '$app/forms';

	export let form;
</script>

<article class="min-h-screen bg-[url(/img/reservation-bg.jpg)] bg-cover bg-center">
	<div class="container mx-auto grid justify-center py-20 px-5 lg:max-w-6xl">
		<section class="top-10 w-full rounded bg-white p-5 shadow md:w-[500px] md:p-16">
			<div class="mb-10 text-center">
				<p class="font-light text-red-400">Reservation</p>
				<h2 class="font-josefin text-3xl font-bold">Book Now</h2>
			</div>

			<form action="" method="POST" class="grid gap-5" use:enhance>
				<!-- Name -->
				<div>
					<label for="" class="text-gray-600">Name</label>
					<input
						type="text"
						name="name"
						class="w-full rounded border border-gray-300 bg-white py-2 px-4 text-gray-600"
						placeholder="Name"
						required
					/>
				</div>

				<!-- Email -->
				<div>
					<label for="" class="text-gray-600">Email</label>
					<input
						type="email"
						name="email"
						required
						class="w-full rounded border border-gray-300 py-2 px-4 text-gray-600"
						placeholder="Email"
					/>
				</div>

				<!-- Phone number -->
				<div>
					<label for="" class="text-gray-600">Phone</label>
					<input
						type="tel"
						name="contact"
						class="w-full rounded border border-gray-300 py-2 px-4 text-gray-600"
						placeholder="Phone"
					/>
				</div>

				<!-- Date -->
				<div>
					<label for="" class="text-gray-600">Date</label>
					<input
						type="date"
						name="date"
						value="2022-12-13"
						required
						class="w-full rounded border border-gray-300 py-2 px-4 text-gray-600"
						placeholder="Date"
					/>
				</div>

				<!-- Time -->
				<div>
					<label for="" class="text-gray-600">Time</label>
					<input
						type="time"
						name="time"
						value="09:30"
						class="w-full rounded border border-gray-300 py-2 px-4 text-gray-600"
						placeholder="Time"
					/>
				</div>

				<!-- No. of people booked -->
				<select
					name="seats"
					class="block w-full rounded border border-gray-300 py-2 px-4 text-gray-600"
				>
					<option value="1" selected>1</option>
					<option value="2">2</option>
					<option value="3">3</option>
					<option value="4">4</option>
					<option value="5">5</option>
				</select>

				<!-- Extra message -->
				<textarea
					name="message"
					class="block min-h-[100px] w-full rounded border border-gray-300 p-2 text-gray-600"
					placeholder="Enter extra things you may need."
				/>

				<!-- Submit button -->
				<div class="text-center">
					<button
						type="submit"
						class="font-open_sans rounded-full bg-red-500 py-2 px-6 text-white shadow-md shadow-red-400"
					>
						Send Message
					</button>
				</div>
			</form>
		</section>
	</div>
</article>

<style></style>
