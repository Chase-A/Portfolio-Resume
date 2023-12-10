<div class="header-container">
    <img src="headshot.png" alt="headshot of me" class="headshot">
    <div class="text-container">
        <div class="left">
            <h1 class="name">Chase Almy</h1>
            <p class="small-text">Process Focused UI/UX Designer</p> 
        </div>
        <div class="contact">
            <p class="small-text">508-654-4390</p>
            <p class="small-text">chaseralmy@gmail.com</p>
            <p class="small-text">Massachusetts (willing to relocate)</p>
        </div>
    </div>
</div>

<style>
    .header-container {
        display: flex;
        max-height: 160px;
    }
    .headshot {
        object-fit: contain;
        max-width: 100px;
    }
    .text-container {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        padding: 12px 0;
        margin-left: 12px;
        border-top: 6px solid black;
        border-bottom: 6px solid black;
        width: 100%;
    }
    .name {
        margin: 2px 0;
        font-size: 36px;
    }
    .small-text {
        margin: 2px 0;
        font-size: 12px;
    }
    @media (min-width: 450px){
        .header-container {
            max-height: 220px;
        }
        .headshot {
            max-width: 140px;
        }
        .name {
            font-size: 48px;
        }
        .small-text {
            font-size: 16px;
        }
    }
    @media only screen and (min-width: 750px){
        .header-container {
            max-height: 160px;
            margin-left: 44px;
        }
        .headshot {
            max-width: 100px;
        }
        .text-container {
            flex-direction: row;
            align-items: center;
            margin-left: 16px;
        }
        .text-container .left {
            margin-bottom: 9px;
        }
        .name {
            margin-bottom: 14px;
        }
        .contact {
            display: flex;
            flex-direction: column;
            gap: 8px;
            text-align: right;
        }
    }
    @media only print and (min-width: 650px){
        .header-container {
            max-height: 160px;
            margin-left: 0px;
        }
        .headshot {
            max-width: 100px;
        }
        .text-container {
            flex-direction: row;
            align-items: center;
            margin-left: 16px;
        }
        .text-container .left {
            margin-bottom: 9px;
        }
        .name {
            margin-bottom: 14px;
        }
        .contact {
            display: flex;
            flex-direction: column;
            gap: 8px;
            text-align: right;
        }
    }
</style>