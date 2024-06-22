<script>
	import '../app.css';
	import { AppBar } from '@skeletonlabs/skeleton';

	let dismissedAlert = false;
</script>

{#if !dismissedAlert}
	<aside class="alert variant-soft-warning">
		<div class="flex w-full flex-row items-center justify-between">
			<span class="mr-4">⚠️</span>
			<span class="flex-grow">
				Hey! This is a portfolio demo.
				<a class="underline" href="https://mccarroll.dev/">Learn more</a>
			</span>
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

<style></style>
