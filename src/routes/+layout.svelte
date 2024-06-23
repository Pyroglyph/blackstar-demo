<script>
	import '../app.css';
	import { AppBar } from '@skeletonlabs/skeleton';
	import { page } from '$app/stores';

	let dismissedAlert = false;
</script>

{#if !dismissedAlert}
	<aside class="alert variant-soft-warning text-sm">
		<div class="flex w-full flex-row items-center justify-between">
			<div class="mr-4">⚠️</div>
			<div class="flex-grow">
				<span class="text-nowrap">Hey! This is a portfolio demo.</span>
				<a class="underline text-nowrap" href="https://mccarroll.dev/">Learn more</a>
			</div>
			<button on:click={() => (dismissedAlert = true)}>✕</button>
		</div>
	</aside>
{/if}

<AppBar slotDefault="mx-auto sm:mx-0 flex flex-col sm:flex-row items-center" gridColumns="1">
	<a href="/" class="mx-auto my-3 sm:mx-0 sm:my-0 sm:inline-block">
		<img src="/logo.svg" alt="Logo" class="h-8" />
	</a>

	<nav class="list-nav flex sm:inline-flex sm:flex-1 sm:justify-end">
		<a class="btn-sm !px-3" href="/about">About</a>
		<a class="btn-sm !px-3" href="/services">Services</a>
		<a class="btn-sm !px-3" href="/careers">Careers</a>
		<a class="btn-sm !px-3" href="/contact">Contact</a>
	</nav>
</AppBar>

<slot></slot>

<footer class="bg-surface-100-800-token inline-block w-full p-4 text-sm sm:p-8">
	<div class="mx-auto flex w-full max-w-screen-lg flex-col sm:flex-row">
		<div class="mb-4 flex-1">
			<h6 class="h6 mb-2">Additional information</h6>
			<p class="mt-2">
				Blackstar International is a fictitious company created for the purpose of this portfolio
				demo. Any resemblance to a real business is purely coincidental.
			</p>
			{#if $page.data.aiUsed}
				<p class="mt-2">
					Generative AI was used to create some of the content on this page. This is because I am a
					developer, not a copy writer.
				</p>
			{/if}
		</div>
		<div class="mb-4 flex-1">
			<h6 class="h6 mb-2">Legal</h6>
			<p class="mt-2">
				All images in this demo are under the
				<a class="underline" href="https://unsplash.com/license">Unsplash License</a>.
			</p>
		</div>
	</div>
	<div class="mb-2 text-center sm:mt-4">
		Like this demo? <a class="underline" href="mailto:connor@mccarroll.dev">Contact me</a>!
	</div>
	<div class="text-center">
		&copy; {new Date().getFullYear()}
		<a href="https://mccarroll.dev/">Connor McCarroll</a>
	</div>
</footer>

<style></style>
