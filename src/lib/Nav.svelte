<script>
    function closeApp() {
        console.log("Close app yay!!!!!!!!!!!!")
    }
</script>

<main>
    <img class="logo" src="bedrockplus.png" alt="Bedrock+">
    <button on:click={closeApp}>
        <img class="exit" src="xmark-solid.svg" alt="">
    </button>
</main>

<style>
    main {
        display: flex;
        position: relative;
        align-items: center;
    }

    .exit {
        fill: white;
        height: 24px;
        width: 24px;
    }

    .logo {
        height: 43px;
        width: 40px;
    }

    button {
        display: flex;
        align-items: center;
        justify-content: center;
        position: absolute;
        right: 15px;
        height: 42px;
        width: 42px;
        background-color: rgba(0, 0, 0, 0.5);
        border: none;
        border-radius: 10px;
        box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
        transition-duration: 250ms;
        backdrop-filter: blur(7.5px); 
    }

    button:active {
        box-shadow: none;
    }
</style>