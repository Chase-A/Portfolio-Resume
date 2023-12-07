<script>
    export let title;
</script>

<div class="entry-container">
    <h2>{title}</h2>
    <p>
        <slot />
    </p>
</div>

<style>
    .entry-container {
        margin-top: 12px;
    }
    h2{
        margin-bottom: 6px;
    }
</style>