<main>
    <div class="why-sponsor-us">
        <div class="title">
            <p>WHY SPONSOR US?</p>
        </div>
        <div class="points">
            <ul>
                <li>Corporate Social Responsibility</li>
                <li>Widespread publicity on social media handles on team & IIITDM</li>
                <li>Kancheepuram, team website, car, banners, giveables</li>
                <li>Media Exposure</li>
                <li>Possible R&D collaboration with IIITDM Kancheepuram</li>
                <li>Supporting Design and Engineering Community</li>
                <li>Helping students to follow their passion</li>
            </ul>
        </div>
        <div class="ending">
            <div class="1">SPONSORSHIP BROCHURE</div>
            <div class="2">COLLABORATE WITH US</div>
            <div class="3">CROWD FUNDING</div>
        </div>
    </div>

    <div class="our-sponsors">
        <div class="title"><p>OUR SPONSORS</p></div>
        <div class="sponsors">
            <div class="sponsor1">DLC</div>
            <div class="sponsor2">DESINGERS CLUB</div>
            <div class="sponsor3">TLC</div>
        </div>
    </div>
</main>

<style>
    main {
        display: grid;
        place-items: center;
        text-align: center;
    }

    .title {
        margin-top: 50px;
    }
    .title p {
        font-family: var(--secondary-font);
        font-size: 3rem;
        background: url('./brushBg.png') center center no-repeat;
        font-weight: 400;
        margin: 10px 0;
    }

    .points {
        width: 60vw;
        margin: 100px auto 50px auto;
        text-align: left;
    }
    .points ul li {
        font-size: 2rem;
        font-weight: lighter;
        list-style: disc;
    }

    .ending {
        width: 100vw;
        font-family: var(--secondary-font);
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        font-size: 2rem;
    }
    .ending div {
        margin: 3rem 6rem;
        width: 250px;
    }

    .our-sponsors {
        margin-top: 100px;
        width: 100vw;
        height: 60vh;
    }

    .our-sponsors .sponsors {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
        font-size: 3rem;
        font-family: var(--secondary-font);
        margin-top: 200px;
    }

    @media (max-width: 800px) {
        .title {
            margin-top: 0;
            background-size: contain;
        }
        .title p {
            padding: 10px;
            font-size: 2rem;
        }

        .points {
            margin-top: 50px;
            width: 80vw;
        }
        .points ul li {
            font-size: 1rem;
        }

        .ending div {
            font-size: 1.5rem;
            margin: 2rem;
        }

        .our-sponsors {
            margin-top: 50px;
            height: 80vh;
        }
        .our-sponsors .sponsors {
            font-size: 2rem;
            margin: 0px;
            height: 80%;
        }
        .our-sponsors .sponsors div {
            align-self: center;
            margin: 2rem;
        }
    }
</style>
