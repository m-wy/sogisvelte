<script>
    import {Card, CardBody, CardTitle, CardSubtitle} from 'sveltestrap/src'

    export let titre;
    export let soustitre;
</script>

<style lang="scss">
    .carte{
      border-radius: 0;
    }

</style>

<Card class="carte m-2">
    <CardBody class="mx-auto">
        <b>{titre}</b>
    </CardBody>
    {#if soustitre != undefined}
        <CardSubtitle class="mx-auto p-2">
            {soustitre}
        </CardSubtitle>
    {/if}
</Card>