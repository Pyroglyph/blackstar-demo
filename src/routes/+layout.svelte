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

<AppBar>
	<img src="/logo.svg" alt="Logo" class="h-12" />
	<svelte:fragment slot="trail">
		<nav class="list-nav flex w-full items-stretch justify-end">
			<a href="/about">About</a>
			<a href="/services">Services</a>
			<a href="/careers">Careers</a>
			<a href="/contact">Contact</a>
		</nav>
	</svelte:fragment>
</AppBar>

<slot></slot>

<style></style>
