<div class="mx-4 my-8 max-w-screen-md sm:mx-auto">
	<h1 class="h1 my-8">Services</h1>
	<div class="grid grid-cols-1 gap-6 sm:grid-cols-2">
		<section>
			<h3 class="h3 mb-3 blue">Strategy and Planning</h3>
			<p>
				Chart a course for success with our expert strategy and planning services. We'll help you
				set goals, prioritize initiatives, and drive results.
			</p>
		</section>
		<section>
			<h3 class="h3 mb-3 red">Technology and IT</h3>
			<p>
				Transform your business with our cutting-edge technology expertise. From cloud migration to
				cybersecurity, we've got you covered.
			</p>
		</section>
		<section>
			<h3 class="h3 mb-3 pink">Project Management</h3>
			<p>
				Get projects done right with our expert project management services. From planning to
				execution, we'll help you deliver on time and on budget.
			</p>
		</section>
		<section>
			<h3 class="h3 mb-3 blue">Business Intelligence</h3>
			<p>
				Unlock the power of your data with our business intelligence expertise. From data analysis
				to visualization, we'll help you unlock the power of your data.
			</p>
		</section>
		<section>
			<h3 class="h3 mb-3 red">Supply Chain Management</h3>
			<p>
				Elevate your supply chain strategy with our strategic consulting, implementation, and
				optimization services, ensuring a competitive edge in the market.
			</p>
		</section>
		<section>
			<h3 class="h3 mb-3 pink">Research and Development</h3>
			<p>
				Drive business growth with our R&D solutions. We'll help you identify opportunities, develop
				new products, and bring them to market quickly and efficiently.
			</p>
		</section>
	</div>

	<div class="card mt-8 p-4 text-center">
		<div class="flex-1">Ready to take your business to the next level?</div>
		<a
			class="variant-filled btn btn-lg mt-4"
			href="mailto:connor@mccarroll.dev?subject=I like your portfolio!"
		>
			Contact us
		</a>
	</div>
</div>

<style lang="less">
	.h3::after {
		@apply relative mt-3 block h-1 w-full bg-gradient-to-r;
		content: '';

		&.blue {
			@apply from-blue-500 to-cyan-300;
		}
		&.red {
			@apply from-red-500 to-yellow-500;
		}
		&.pink {
			@apply from-pink-500 to-violet-500;
		}
	}
</style>
