<script lang="ts">
	export let profile: any;
</script>

<div class="w-full h-1/6 flex">
	<div class="w-5/12 h-full flex flex-col justify-center pl-2">
		<h1 class="text-lg">
			{profile.name}
		</h1>
		<h2>
			{profile.title}
		</h2>
		<h3>
			{profile.birthplace}
		</h3>
	</div>
	<div class="w-2/12 h-full flex flex-col justify-center">
		<img
			class="profile-picture w-11/12 rounded-full border-[#449399] border-[4px]"
			src="/profile.jpg"
			alt=""
		/>
	</div>
	<div class="w-5/12 flex h-full">
		<div class="text-right flex flex-col justify-center ml-1 text-xs ">
			<div class="flex justify-end">
				<h5>{profile.email}</h5>
				<span class=" w-[20px] flex justify-center"><i class="fas fa-envelope " /></span>
			</div>
			<div class="flex justify-end">
				<h5>{profile.phone}</h5>
				<span class=" w-[20px] flex justify-center"><i class="fas fa-mobile-alt " /></span>
			</div>
			<div class="flex justify-end">
				<h5>{profile.address}</h5>
				<span class=" w-[20px] flex justify-center"><i class="fas fa-map-marker-alt " /></span>
			</div>
	 
		</div>
	</div>
</div>
