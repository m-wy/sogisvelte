
<script>
    import {_, locale, locales} from 'svelte-i18n';
    import {Button, Col, Row} from 'sveltestrap/src'
    export let titre;
    export let contenu;
</script>

<style>

</style>

<h2>
    {@html titre}
</h2>
{#if contenu != undefined}
<p>
    {@html contenu}
</p>
{/if}