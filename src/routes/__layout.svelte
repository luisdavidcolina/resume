<script lang="ts">
	import '../app.css';
	import PageWhite from '../components/elements/PageWhite.svelte';
</script>

<div class="w-screen h-screen bg-black">
	<PageWhite>
		<slot />
	</PageWhite>
</div>
