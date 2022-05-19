<script lang="ts">
	export let profile: any;
	export let lenguaje: string;
</script>

<div class="w-full flex-1">
	<h3>{lenguaje === 'es' ? 'REFERENCIAS' : 'PERSONAL REFERENCES'}</h3>
	{#each profile.personalReferences as reference}
		<h5>
			{reference.name} - {reference.title}
		</h5>
		<h6>
			Contacto: {reference.phone}
		</h6>
	{/each}
</div>
