<script>
	import App from "../node_modules/@sapper/internal/App.svelte";
</script>
<svelte:head>
	<title>About</title>
</svelte:head>

<h1>About this site</h1>

<p>This is the 'about' page. There's not much here.</p>
<button on:click>Click me</button>

<style lang="scss">

	$primary: red;

	button {
		color: $primary;
	}
</style>

