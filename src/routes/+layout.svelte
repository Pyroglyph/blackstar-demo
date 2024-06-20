<script>
	import '../app.css';
	import { AppBar } from '@skeletonlabs/skeleton';

	let dismissedAlert = false;
</script>

{#if !dismissedAlert}
	<aside class="alert variant-soft-warning">
		<div class="flex w-full flex-row items-center justify-between">
			<span>⚠️ Hey! This is a demo site, and therefore does not represent a real company.</span>
			<button on:click={() => (dismissedAlert = true)}>✕</button>
		</div>
	</aside>
{/if}

<AppBar slotDefault="mx-auto sm:mx-0 flex flex-col sm:flex-row items-center" gridColumns="1">
	<a href="/" class="mx-auto my-3 sm:mx-0 sm:my-0 sm:inline-block">
		<img src="/logo.svg" alt="Logo" class="h-8" />
	</a>

	<nav class="list-nav flex sm:inline-flex sm:flex-1 sm:justify-end">
		<a href="/about">About</a>
		<a href="/services">Services</a>
		<a href="/careers">Careers</a>
		<a href="/contact">Contact</a>
	</nav>
</AppBar>

<slot></slot>

<style></style>
