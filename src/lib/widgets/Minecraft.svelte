<script>
    export let name, date

    function settings() {
        console.log("settings menu opened yes")
    }
</script>

<main>
    <h1>{name}</h1>
    <div class="tags">
        <div>{date}</div>
        <div on:click={settings} class="settings">
            <img src="gear-solid.svg" alt="">
        </div>
    </div>
</main>

<style>
    main {
        border-radius: 25px;
        background: linear-gradient(90deg, rgba(0, 0, 0, 0.4) 0%, rgba(0, 0, 0, 0.4) 100%), url(/minecraft_background.png);
        background-size: cover;
        background-repeat: no-repeat;
        padding: 2px;
        padding-bottom: 5px;
        padding-left: 15px;
        padding-top: 15px;
    }

    div img {
        height: 16px;
        width: 16px;
    }

    .tags {
        display: flex;
        flex-direction: row;
        gap: 5px;
    }

    .tags div {
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: rgba(0, 0, 0, 0.5);
        backdrop-filter: blur(7.5px);
        width: fit-content;
        padding: 2px;
    }

    .settings {
        height: 24px;
        width: 24px !important;
    }

    .settings img {
        height: 12px;
        width: 12px;
    }

    h1 {
        font-weight: 900;
        width: 10rem;
        margin: 0px;
        line-height: 2.25rem;
        margin-bottom: 15px;
    }
</style>