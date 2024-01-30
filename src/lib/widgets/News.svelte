<script>
    export let title, url
</script>

<main>
    <h1>{title}</h1>
    <slot/>
    <br>
    <br>
    <a href={url}>Read More</a>
</main>

<style>
    main {
        background-color: rgba(0, 0, 0, 0.5);
        height: fit-content;
        width: fit-content;
        padding: 20px;
        border-radius: 15px;
        backdrop-filter: blur(7.5px); 
    }

    h1 {
        font-size: 24px;
    }

    a {
        font-size: 24px;
        color: white;
        text-decoration: none;
        background-color: rgba(53, 142, 225, 0.42);
        padding: 5px;
        padding-left: 64px;
        padding-right: 64px;
        border-radius: 15px;
        box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25); 
    }
</style>