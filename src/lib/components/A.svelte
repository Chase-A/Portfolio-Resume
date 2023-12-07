<script>
    export let url;
</script>

<a href="{url}" target="_blank" rel="noopener noreferrer"><slot /></a>

<style>
    a {
        color: #000;
        font-weight: 700;
    }
    a:hover {
        color: #777;
    }
</style>