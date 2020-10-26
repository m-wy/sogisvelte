<footer>
<ul class="lang">
    {#each $locales as item}
        <li>
        <span
                class="a"
                class:selected={$locale.includes(item)}
                href={`#!${item}`}
                on:click={() => ($locale = item)}>
          {$_('languages.' + item.replace('-', '_'))}
        </span>
        </li>
    {/each}
</ul>
</footer>

<script>
    import { _, locale, locales } from 'svelte-i18n';
</script>