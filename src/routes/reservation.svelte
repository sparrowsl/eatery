<script>
	import { goto } from '$app/navigation';
	import { formSuccess } from '../lib/store.js';

	const customer = {
		name: '',
		email: '',
		phone: '',
		date: '',
		time: '09:30',
		people: '',
		message: ''
	};

	const handleForm = () => {
		$formSuccess = true;
		goto('/');
	};
</script>

<article class="min-h-screen bg-[url(/img/reservation-bg.jpg)]">
	<div class="container mx-auto grid justify-center py-20 px-5 lg:max-w-6xl">
		<section class="top-10 w-full rounded bg-white p-5 shadow md:w-[500px] md:p-16">
			<div class="mb-10 text-center">
				<p class="font-light text-red-400">Reservation</p>
				<h2 class="font-josefin text-3xl font-bold">Book Now</h2>
			</div>

			<form action="" class="grid gap-5" on:submit|preventDefault={handleForm}>
				<!-- Name -->
				<div>
					<label for="" class="text-gray-600">Name</label>
					<input
						bind:value={customer.name}
						type="text"
						class="w-full rounded border-[1px] border-gray-300 bg-white py-2 px-4 text-gray-600"
						placeholder="Name"
						required
					/>
				</div>
				<!-- Email -->
				<div>
					<label for="" class="text-gray-600">Email</label>
					<input
						bind:value={customer.email}
						type="email"
						required
						class="w-full rounded border-[1px] border-gray-300 py-2 px-4 text-gray-600"
						placeholder="Email"
					/>
				</div>
				<!-- Phone number -->
				<div>
					<label for="" class="text-gray-600">Phone</label>
					<input
						bind:value={customer.phone}
						type="tel"
						class="w-full rounded border-[1px] border-gray-300 py-2 px-4 text-gray-600"
						placeholder="Phone"
					/>
				</div>
				<!-- Date -->
				<div>
					<label for="" class="text-gray-600">Date</label>
					<input
						bind:value={customer.date}
						type="date"
						required
						class="w-full rounded border-[1px] border-gray-300 py-2 px-4 text-gray-600"
						placeholder="Date"
					/>
				</div>
				<!-- Time -->
				<div>
					<label for="" class="text-gray-600">Time</label>
					<input
						bind:value={customer.time}
						type="time"
						class="w-full rounded border-[1px] border-gray-300 py-2 px-4 text-gray-600"
						placeholder="Time"
					/>
				</div>
				<!-- No. of people booked -->
				<div>
					<select
						on:change={(e) => (customer.people = e.target.value)}
						class="w-full rounded border-[1px] border-gray-300 py-2 px-4 text-gray-600"
					>
						<option value="" hidden>Persons</option>
						<option value="1">1</option>
						<option value="2">2</option>
						<option value="3">3</option>
						<option value="4">4</option>
						<option value="5">5</option>
					</select>
				</div>
				<!-- Extra message -->
				<div>
					<textarea
						bind:value={customer.message}
						class="min-h-[100px] w-full rounded border-[1px] border-gray-300 p-2 text-gray-600"
						placeholder="Enter extra things you may need."
					/>
				</div>

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
