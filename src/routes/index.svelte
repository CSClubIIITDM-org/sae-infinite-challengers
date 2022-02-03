<script>
    import About from "/src/components/About.svelte";
    // import Saos from 'saos';
</script>

<main>
    <div class="first-half">
        <div class="title">
            <p>INFINITE</p>
            <p>CHALLENGER</p>
        </div>

        <div class="challenging-the-infinity">
            <p>Challenging The Infinity</p>
            <img src="/static/index/keyboard_arrow_down.svg" alt="">
        </div>
    </div>

    <!-- <Saos animation={'from-bottom 1s cubic-bezier(0.35, 0.5, 0.65, 0.95)'} once={true}> -->
        <section class="About" id="about">
            <About/>
        </section>
    <!-- </Saos> -->
</main>

<style>
    main {
        display: flex;
        flex-direction: column;
        /* justify-content: center; */
        align-items: center;
        text-align: center;
    }
    
    .first-half {
        display: grid;
        justify-content: center;
        width: 100vw;
        height: 100vh;
    }
    .title {
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        margin-top: 50px;
        width: 60vw;
        height: 35vw;
        background: url('/static/index/car.png') center center no-repeat;
        background-size: 80%;
    }
    .title p {
        margin: 5vw 0 5vw 0;
        font-family: var(--secondary-font);
        font-size: 8vw;
        text-shadow: 0px 10px 10px gray;
    }

    .challenging-the-infinity p {
        font-size: 3rem;
        color: var(--secondary-text-color);
    }

    @media (max-width: 800px) {
        .first-half {
            height: 93vh;
            display: flex;
            flex-direction: column;
            justify-content: space-around;
            align-items: center;
        }

        .title {
            /* border: solid red; */
            width: 100vw;
            height: 50vh;
            background-size: 100%;
        }

        .title p {
            font-size: 10vw;
        }

        .challenging-the-infinity p {
            font-size: 2rem;
        }
        .challenging-the-infinity img {
            width: 4rem;
        }
    }
</style>
