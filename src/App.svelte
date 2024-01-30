<script>
    import Nav from "./lib/Nav.svelte";
    import Changelog from "./lib/widgets/Changelog.svelte";
    import Launch from "./lib/widgets/Launch.svelte";
    import Minecraft from "./lib/widgets/Minecraft.svelte";
    import News from "./lib/widgets/News.svelte";

    
</script>

<main>
    <Nav/>
    <div class="content">
        <div class="minecraft">
            <Minecraft name="Minecraft 1.19.20" date="11.9.2001"/>
            <Changelog>
                [+] Release v1.0.0<br>
                [+] Release v1.0.0<br>
                [+] Release v1.0.0<br>
                [+] Release v1.0.0<br>
                [+] Release v1.0.0<br>
                [+] Release v1.0.0<br>
            </Changelog>
            <Launch/>
        </div>
        <div class="news">
            <News title="Is the news cool?" url="https://youtube.com/">
                test<br>
                test<br>
                test<br>
                test
            </News>
        </div>
    </div>
</main>

<style>
    main {
        padding-top: 25px;
        padding-left: 20px;
        padding-right: 20px;
    }

    .content {
        display: flex;
        flex-direction: row;
        gap: 25px;
    }

    .news {

    }

    .minecraft {
        display: flex;
        flex-direction: column;
        gap: 10px;
    }
</style>
