<script>
    import About from "/src/components/About.svelte";
    import Saos from 'saos';
</script>

<main>
    <div class="first-half">
        <div class="title">
            <p>INFINITE<br>CHALLENGER</p>
        </div>

        <div class="challenging-the-infinity">
            <p>Challenging The Infinity</p>
        </div>
        <img src="/static/index/keyboard_arrow_down.svg" alt="">
    </div>

    
    <section class="About" id="about">
        <Saos animation={'from-bottom 1s cubic-bezier(0.35, 0.5, 0.65, 0.95)'}>
            <div class="blank"></div>
            <About/>
        </Saos>
    </section>
</main>

<style>
    main {
        text-align: center;
    }

    .first-half {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 100vw;
        height: 100vh;
    }
    .title {
        margin-top: 120px;
        background: url('/static/index/car.png') center center no-repeat;
        background-size: 40rem auto;
    }
    .title p {
        line-height: 15rem;
        font-family: var(--secondary-font);
        font-size: 6rem;
        text-shadow: 0px 0px 10px gray;
    }

    .challenging-the-infinity p {
        margin: 6rem 0;
        font-size: 2.5rem;
        font-weight: bold;
        color: var(--secondary-text-color);
    }
    .first-half img {
        position: absolute;
        left: 0;
        right: 0;
        margin-left: auto;
        margin-right: auto;
        bottom: 15px;
        animation: arrow-animation 1.5s infinite;
    }

    @keyframes arrow-animation {
        0% {
            transform: translateY(0);
            opacity: 0;
        }
        50% {
            opacity: 1;
        }
        100% {
            transform: translateY(20px);
            opacity: 0;
        }
    }

    #about .blank {
        width: 100vw;
        height: 10vh;
    }

    @media (max-width: 900px) {
        .title {
            background-size: 40rem auto;
        }
        .title p {
            line-height: 15rem;
            font-size: 5rem;
        }

        .challenging-the-infinity p {
            margin: 5rem 0 7rem 0;
            font-size: 2.5rem;
        }
        .first-half img {
            width: 80px;
        }
    }

    @media (max-width: 650px) {
        .title {
            background-size: 25rem auto;
        }
        .title p {
            line-height: 9rem;
            font-size: 3rem;
        }
        .challenging-the-infinity p {
            margin: 4rem 0 5rem 0;
            font-size: 1.8rem;
        }
    }
</style>
