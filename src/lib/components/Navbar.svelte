<script>
    import { page } from '$app/stores';
    let links = ['Portfolio', 'Resume', 'About']
    let currentPage = $page.url.pathname.split('/').pop();
    console.log(currentPage)
</script>

<nav class="nav-container">
    {#each links as link}
        <a class="link" href="/{link === 'Portfolio' ? '': link.toLowerCase()}">{link}</a>
    {/each}
</nav>

<style>
    .nav-container {
        display: flex;
        gap: 4px;
        margin-top: 12px;
    }
    .link {
        text-decoration: none;
        color: black;
        font-weight: bold;
        border: 2px solid black;
        width: 33.33333333%;
        text-align: center;
        padding: 8px 0;
    }
    .link:hover {
        background: #000;
        color: #fff;
    }
    .highlighted {
        background: #000;
        color: #fff;
    }
    @media (min-width:700px){
        .nav-container {
            flex-direction: column;
            margin-right: 16px;
            margin-top: 16px;
        }
        .link {
            width: 140px;
        }
    }
</style>