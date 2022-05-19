<script lang="ts"> 
</script>
<div class="page m-auto bg-white flex flex-col px-4">
	<div class="nada">
		<span class="square" />
		<span class="square2" />
		<span class="square3" />
		<span class="square4" />
		<span class="square5" />
	</div>
	<slot />
</div>

<style>
	.page {
		height: calc(525px * (3508 / 2480));
		max-width: 550px;
	}
	.nada {
		position: absolute;
		margin-left: -16px;
	}
	.square {
		height: 5vh;
		width: 1.2vw;
		background-color: #313c4e;
		position: absolute;
		margin-top: 4vh;
		left: 0;
	}
	.square2 {
		height: 5vh;
		width: 1.2vw;
		background-color: #449399;
		position: absolute;
		top: 20vh;
	}
	.square3 {
		height: 5vh;
		width: 1.2vw;
		background-color: #449399;
		position: absolute;
		top: 41vh;
	}
	.square4 {
		height: 5vh;
		width: 1.2vw;
		background-color: #449399;
		position: absolute;
		top: 61vh;
	}
	.square5 {
		height: 5vh;
		width: 1.2vw;
		background-color: #449399;
		position: absolute;
		top: 81vh;
	}
</style>
