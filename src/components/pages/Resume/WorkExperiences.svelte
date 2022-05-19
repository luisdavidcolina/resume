<script lang="ts">
	export let profile: any;
	export let lenguaje: string;
</script>

<h3>{lenguaje === 'es' ? 'EXPERENCIA LABORAL' : 'WORK EXPERIENCES'}</h3>
{#each profile.workExperiences as workExperience}
	<div class="mb-2 ">
		<h4>
			{workExperience.title}
		</h4>
		<h5>
			{workExperience.company}
		</h5>
		<h6 class="flex justify-between">
			<span>
				{workExperience.startDate} - {workExperience.endDate}
			</span>
			<span>
				{workExperience.location}
			</span>
		</h6>
		<p class="text-justify">
			{workExperience.description}
		</p>
		<h6>Responsabilidades</h6>

		<ul class=" ">
			{#each workExperience.responsibilities as responsibilitie}
				<li class="text-justify">
					{responsibilitie}
				</li>
			{/each}
		</ul>
	</div>
{/each}
