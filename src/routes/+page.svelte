<script lang="ts">
</script>

<div class="container mx-auto my-16">
	<div class="mx-auto my-16 w-48 text-center lg:my-32">
		<h1 class="hero-gradient from-blue-500 to-cyan-300">Design.</h1>
		<h1 class="hero-gradient from-red-500 to-yellow-500">Adapt.</h1>
		<h1 class="hero-gradient from-pink-500 to-violet-500">Deliver.</h1>
	</div>
	<div class="card m-4 flex flex-col items-center p-8 sm:m-8 sm:mx-auto sm:flex-row">
		<div>
			<p>
				We are the world's most effective consulting group. With over 3,000 projects completed, we
				will find innovative solutions for your business.
			</p>
			<p>
				We are <strong>BLACKSTAR</strong>.
			</p>
		</div>

		<button class="variant-filled btn btn-lg mt-8 sm:ml-8 sm:mt-0">Learn more</button>
	</div>
</div>
<div class="collab-image flex items-center justify-center">
	<div
		class="card variant-glass-surface h2 mx-4 mb-32 mt-48 w-auto p-4 text-center text-white sm:mb-48 sm:mt-96 sm:p-8"
	>
		<span class="text-nowrap">Working with you,</span>
		<span class="text-nowrap">every step of the way.</span>
	</div>
</div>

<style lang="less">
	.hero-gradient {
		@apply h1 bg-gradient-to-br box-decoration-clone bg-clip-text text-transparent;

		font-size: 3rem;
		line-height: 3.8rem;
	}

	.collab-image {
		@apply w-full bg-cover bg-center bg-no-repeat;
		background: url('https://images.unsplash.com/photo-1543269865-cbf427effbad?q=80&w=1920&auto=format&fit=crop')
			center center / cover no-repeat;
	}
</style>
