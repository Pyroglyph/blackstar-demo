<script lang="ts">
	import { mailtoLink } from '$lib/utils';
</script>

<div class="mx-4 my-8 max-w-screen-md sm:mx-auto">
	<h1 class="h1 my-8">Careers</h1>
	<div class="grid grid-cols-1 gap-4 sm:grid-cols-2">
		<p>
			We are always looking for talented individuals to join our team. If you are passionate about
			technology and innovation, we want to hear from you. We offer competitive salaries, flexible
			work hours, and a supportive work environment.
		</p>
		<div class="card grid gap-4 p-4">
			<p>
				If you are interested in joining our team, please send us your resume and cover letter:
				<a href={mailtoLink} class="mx-auto mt-2 block text-center underline">
					careers@blackstar.international
				</a>
			</p>
		</div>
		<p>We look forward to working with you!</p>
	</div>
</div>
