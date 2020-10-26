<script>
	import { _ } from 'svelte-i18n'</script>
<svelte:head>
	<title>About</title>
</svelte:head>

<h1>About this site</h1>

<p>This is the 'about' page. There's not much here.</p>
<button on:click>{$_('title.index')}</button>

<style lang="scss">

	$primary: red;

	button {
		color: $primary;
	}
</style>

