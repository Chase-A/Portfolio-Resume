<script>
    import "../app.css"
    import Header from "../lib/components/Header.svelte";
    import Navbar from "../lib/components/Navbar.svelte";
</script>

<Header />
<div class="body-container">
    <Navbar />
    <div>
       <slot /> 
    </div>
</div>

<style>
    @media (min-width: 700px){
        .body-container {
            display: flex;
        }
    }
</style>