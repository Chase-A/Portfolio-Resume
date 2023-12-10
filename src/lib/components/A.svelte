<script>
    export let url;
    export let newTab = true;
</script>

{#if newTab}
    <a href="{url}" target="_blank" rel="noopener noreferrer"><slot /></a>
{:else}
    <a href="{url}"><slot /></a>
{/if}

<style>
    a {
        color: #000;
        font-weight: 700;
    }
    a:hover {
        color: #777;
    }
</style>