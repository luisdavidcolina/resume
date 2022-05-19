<script lang="ts">
	export let lenguaje: string;
</script>

<label class="swap swap-rotate">
	<input
		type="checkbox"
		checked={lenguaje !== 'es'}
		on:click={() => {
			lenguaje = lenguaje === 'es' ? 'en' : 'es';
			console.log(lenguaje);
		}}
	/>
	<div class="swap-off fill-current w-10 h-10">ESP</div>
	<div class="swap-on fill-current w-10 h-10">ENG</div>
</label>
<a href="luisdavidcolina.pdf" target="_blank">
	<i class="fas fa-file-download" />
</a>

<style>
	.swap {
		position: absolute;
		left: 1vw;
		top: 1vh;
		z-index: 2;
		color: #fff;
	}

	.fa-file-download {
		height: 20px;
		width: 20px;
		position: absolute;
		left: 1vw;
		top: 7vh;
		z-index: 2;
		color: #fff;
	}
</style>
