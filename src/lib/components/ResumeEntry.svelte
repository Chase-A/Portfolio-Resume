<script>
    export let title;
    export let startDate;
    export let  endDate;
</script>

<div class="resume-entry">
    <h2 class="title">{title}</h2>
    <p class="dates">{startDate} - {endDate}</p>
    <ul class="points">
        <slot />
    </ul>
</div>

<style>
    .resume-entry {
        margin-top: 12px;
    }
    .title {

    }
    .dates {
        font-size: 12px;
    }
    .points {
        margin-top: 6px;
        list-style-type: square;
        padding-left: 20px;
    }
</style>