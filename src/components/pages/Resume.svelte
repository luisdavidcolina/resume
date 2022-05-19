<script lang="ts">
	import TechStack from './Resume/TechStack.svelte';
	import WorkExperiences from './Resume/WorkExperiences.svelte';
	import MainInformation from './Resume/MainInformation.svelte';
	import SwapLenguaje from '../elements/SwapLenguaje.svelte';
	import SoftSkills from './Resume/SoftSkills.svelte';
	import Education from './Resume/Education.svelte';
	import { profileES, profileEN } from '../../data';
	import PersonalReferences from './Resume/PersonalReferences.svelte';
	import OtherProjects from './Resume/OtherProjects.svelte';

	let lenguaje = 'es';
	$: profile = lenguaje === 'es' ? profileES : profileEN;
</script>

<SwapLenguaje bind:lenguaje />

<MainInformation {profile} />

<div class="w-full mb-4 border-[#449399] border-b-[3px]" />

<div class="w-full flex-1 flex ">
	<div class="w-1/2 px-2 flex-col ">
		<WorkExperiences {lenguaje} {profile} />
		<OtherProjects {lenguaje} {profile} />
	</div>
	<div class="w-1/2 flex flex-col px-2">
		<Education {lenguaje} {profile} />
		<TechStack {lenguaje} {profile} />
		<SoftSkills {lenguaje} {profile} />
		<PersonalReferences {lenguaje} {profile} />
	</div>
</div>
