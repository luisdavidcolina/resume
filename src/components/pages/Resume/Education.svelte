<script lang="ts">
	export let profile: any;
	export let lenguaje: string;
</script>

<div class="w-full flex-1 mb-5">
	<h3>{lenguaje === 'es' ? 'FORMACIÓN ACADÉMICA' : 'EDUCATION'}</h3>
	{#each profile.education as education}
		<div class="mb-2">
			<h4>
				{education.title}
			</h4>
			<h5>
				{education.institution}
			</h5>
			<h6 class="flex justify-between">
				<span>
					{education.startDate} - {education.endDate}
				</span>
				<span>
					{education.location}
				</span>
			</h6>
			<div class="flex">
				<span class="w-1/2">
					<ul>
						{#each education.courses.slice(0, 3) as course}
							<li class="mr-3">
								{course}
							</li>
						{/each}
					</ul>
				</span>
				<span class="w-1/2">
					<ul>
						{#each education.courses.slice(3, 6) as course}
							<li class="mr-3">
								{course}
							</li>
						{/each}
					</ul>
				</span>
			</div>
		</div>
	{/each}
	<h4>Otros cursos</h4>
	<h6 class="">
		Diseño de interfaces y experiencias de usuario. Seguridad informática. Inteligencia artificial.
	</h6>
</div>
