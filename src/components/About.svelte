<section class="about-us">
    <div class="about-us__title">
        <p>About Us</p>
    </div>
    
    <div class="about-us__stats">
        <div class="about-us__stats1">
            <h1><b>25+</b></h1>
            <p>Students</p>
        </div>
        <div class="about-us__stats2">
            <h1><b>6+</b></h1>
            <p>Specializations</p>
        </div>
        <div class="about-us__stats3">
            <h1><b>1</b></h1>
            <p>Goal</p>
        </div>
    </div>

    <div class="about-us__content">
        <p>The IIITDM Kancheepuram SAE Baja team also known as Team Infinite Challengers, a student organization of  25 interdisciplinary engineers. Our team consists of different departments like Roll cage, Suspension, Steering, Brakes, Electronics and Transmission & Powertrain. We have been mentored by two expert faculties, Dr. Shubhankar Chakraborty and Dr. Kashfull Orra.</p>
    </div>

    <div class="about-us__ending">
        <p>FEEL THE ADRENALINE RUSH</p>
    </div>
</section>

<style>
    .about-us {
        width: 100vw;
        display: grid;
        align-items: center;
    }
    .about-us .about-us__title {
        margin: 0 auto;
    }
    .about-us .about-us__title p {
        padding: 10px;
        font-family: var(--secondary-font);
        font-size: 3rem;
		background: url('./brushBg.png') no-repeat center center;
        background-size: contain;
    }

    .about-us__stats {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
        align-items: center;
        margin: 4rem 0;
        height: 350px;
        background: linear-gradient(rgba(0, 0, 0, 0.67), rgba(0, 0, 0, 0.67)), url('/static/index/background-rectangle.png') center center no-repeat;
    }
    .about-us__stats div {
        padding: 20px;
    }
    .about-us__stats h1 {
        font-size: 3.5rem;
    }
    .about-us__stats p {
        font-size: 2.5rem;
    }
    .about-us__content {
        width: 91vw;
        margin: 0 auto;
    }
    .about-us__content p {
        font-size: 1.5rem;
    }

    .about-us__ending {
        margin: 4rem 0 7rem 0;
        padding: 10px;
        background-size: contain;
    }
    .about-us__ending p {
        font-size: 2.5rem;
        font-family: var(--primary-font);
        color: var(--primary-accent-color);
        font-weight: bold;
    }

    @media (max-width: 900px) {
        .about-us .about-us__title p {
            font-size: 3rem;
        }

        .about-us__stats {
            width: 100vw;
            margin: 3rem auto;
            display: flex;
            flex-direction: row;
            justify-content: space-around;
        }

        .about-us__content {
            margin-top: 0;
        }
        .about-us__content p {
            font-size: 1.3rem;
        }

        .about-us__ending {
            margin: 50px auto 100px auto;
        }
        .about-us__ending p {
            font-size: 2rem;
        }
    }

    @media (max-width: 650px) {
        .about-us__stats h1 {
            font-size: 2rem;
        }
        .about-us__stats p {
            font-size: 1.5rem;
        }
        .about-us__stats {
            flex-direction: column;
            justify-content: space-around;
            background: none;
            height: auto;
            background: linear-gradient(145deg, #141414, #181818);
            box-shadow: 12px 12px 33px #101010, -12px -12px 33px #1c1c1c;
            border-radius: 2rem;
            width: auto;
            margin: 2rem;
        }
        .about-us__content {
            margin: 0 auto;
        }
    }
</style>