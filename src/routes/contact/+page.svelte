<script lang="ts">
	import { getToastStore } from '@skeletonlabs/skeleton';
	import type { ToastSettings, ToastStore } from '@skeletonlabs/skeleton';

	const toastStore = getToastStore();

	function submitForm() {
		toastStore.trigger({
			message: 'If this was a real website, your message would have been sent!',
			classes: 'bg-success-500 text-white',
		});
	}
</script>

<div class="mx-4 my-8 max-w-screen-md sm:mx-auto">
	<h1 class="h1 my-8">Contact</h1>
	<p class="mb-2">Have a question or want to learn more about our services?</p>
	<p class="mb-8">Send us a message and we will get back to you as soon as possible.</p>
	<form class="grid columns-1 grid-cols-1 gap-4 sm:grid-cols-2">
		<div class="form-group">
			<label for="name" class="mb-1">Name</label>
			<input type="text" id="name" name="name" class="input px-2 py-1" />
		</div>
		<div class="form-group">
			<label for="email" class="mb-1">Email</label>
			<input type="email" id="email" name="email" class="input px-2 py-1" />
		</div>
		<div class="form-group">
			<label for="company" class="mb-1">Company</label>
			<input type="text" id="company" name="company" class="input px-2 py-1" />
		</div>
		<div class="form-group">
			<label for="job-title" class="mb-1">Job title</label>
			<input type="text" id="job-title" name="job-title" class="input px-2 py-1" />
		</div>
		<div class="form-group sm:col-span-2">
			<label for="message" class="mb-1">Message</label>
			<textarea id="message" name="message" class="input px-2 py-1"></textarea>
		</div>
		<button type="submit" class="variant-filled btn sm:col-span-2" on:click={submitForm}>
			Send
		</button>
	</form>
</div>
