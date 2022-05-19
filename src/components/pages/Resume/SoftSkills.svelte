<script lang="ts">
	export let profile: any;
	export let lenguaje: string;
</script>

<div class="w-full flex-1">
	<h3>{lenguaje === 'es' ? 'HABILIDADES BLANDAS' : 'SOFT SKILLS'}</h3>
	<div class="break-words">
		{#each profile.softSkills as softSkill}
			<span
				class="truncate badges text-white text-xs font-semibold mr-1 py-0.5 rounded dark:bg-pink-200 dark:text-pink-900"
				>{softSkill}</span
			>
		{/each}
	</div>
</div>
