<script>
	import Saos from 'saos';
	import { onMount } from 'svelte';
	onMount(() => {
		const brouchure = document.querySelector('.brouchure');
		const overlay = document.querySelector('.overlay');
		const brouchureButton = document.querySelector('.brouchure-button');
		brouchureButton.addEventListener('click', () => {
			overlay.classList.remove('hidden');
			brouchure.classList.remove('hidden');
		});
		overlay.addEventListener('click', () => {
			console.log('1211');
			overlay.classList.add('hidden');
			brouchure.classList.add('hidden');
		});
	});
</script>

<svelte:head>
	<title>Infinite Challenger | Sponsers</title>
</svelte:head>

<main>
	<Saos animation={'from-bottom 1s cubic-bezier(0.35, 0.5, 0.65, 0.95)'}>
		<div class="why-sponsor-us">
			<div class="title">
				<p>WHY SPONSOR US?</p>
			</div>
			<div class="points">
				<ul>
					<li>Corporate Social Responsibility</li>
					<li>
						Widespread publicity on social media handles on team & IIITDM Kancheepuram, team
						website, car, banners, giveables
					</li>
					<li>Media Exposure</li>
					<li>Possible R&D collaboration with IIITDM Kancheepuram</li>
					<li>Supporting Design and Engineering Community</li>
					<li>Helping students to follow their passion</li>
				</ul>
			</div>
			<div class="brouchure-container">
				<div class="brouchure-button">SPONSORSHIP BROCHURE</div>
			</div>
			<div class="ending">
				<div class="2">COLLABORATE WITH US</div>
				<div class="3">CROWD FUNDING</div>
			</div>
		</div>

		<div class="our-sponsors">
			<div class="title"><p>OUR SPONSORS</p></div>
			<div class="sponsors">
				<div class="sponsor">
					<p>DIC</p>
					<img src="./sponsors/DIC.svg" alt="DIC" />
				</div>
				<div class="sponsor">
					<p>DESINGERS CLUB</p>
					<img src="./sponsors/iiitdm.svg" alt="Desingers_Club" />
				</div>
				<div class="sponsor">
					<p>TLC</p>
					<img src="./sponsors/TLC.svg" alt="TLC" />
				</div>
				<div class="sponsor">
					<p>IIITDM Alumini</p>
					<img src="./sponsors/iiitdm.svg" alt="TLC" />
				</div>
				<div class="sponsor">
					<p>Koshi Motors</p>
					<img src="./sponsors/koshi.jpeg" alt="TLC" />
				</div>
				<div class="sponsor">
					<p>HDFC Bank</p>
					<img src="./sponsors/hdfc.jpeg" alt="TLC" />
				</div>
				<div class="sponsor">
					<p>Indian Bank, Allahabad</p>
					<img src="./sponsors/allahabad.jpeg" alt="TLC" />
				</div>
				<div class="sponsor">
					<p>Scolarian Racing</p>
					<img src="./sponsors/scolarian.png" alt="TLC" />
				</div>
			</div>
		</div>
	</Saos>
	<div class="overlay hidden" />
	<div class="brouchure hidden">
		<embed src="./brouchure.pdf" type="application/pdf" />
	</div>
</main>

<style>
	main {
		display: grid;
		place-items: center;
		text-align: center;
		position: relative;
	}

	.title {
		margin-top: 100px;
	}
	.title p {
		font-family: var(--primary-font);
		font-size: 4rem;
		font-style: italic;
		color: var(--primary-accent-color);
		font-weight: bold;
		margin: 10px 0;
	}

	.points {
		width: 70vw;
		margin: 100px auto;
		text-align: left;
	}
	.points ul li {
		font-size: 2rem;
		font-weight: lighter;
		list-style: disc;
	}

	.ending,
	.brouchure-container {
		width: 80vw;
		font-family: var(--secondary-font);
		display: flex;
		flex-wrap: wrap;
		justify-content: space-evenly;
		align-items: center;
		font-size: 2rem;
	}
	.ending div,
	.brouchure-button {
		border-radius: 1rem;
		padding: 2rem;
		margin: 1rem;
		width: 250px;
		cursor: pointer;
	}
	.brouchure-button {
		box-shadow: 12px 12px 33px #000000, -12px -12px 33px #2c2c2c;
	}
	.ending div:hover {
		transition: all 0.3s;
		box-shadow: 12px 12px 33px #101010, -12px -12px 33px #1c1c1c;
	}

	.our-sponsors {
		margin: 100px auto;
		width: 80vw;
	}

	.our-sponsors .sponsors {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-evenly;
		font-size: 3rem;
		font-family: var(--primary-font);
		margin: 100px auto;
		display: flex;
		justify-content: space-around;
		align-items: baseline;
	}
	.sponsors div {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: space-between;
		height: 300px;
		padding: 50px;
		border-radius: 2rem;
		transition: all 0.3s;
	}
	.sponsors div:hover {
		background: linear-gradient(145deg, #141414, #181818);
		box-shadow: 12px 12px 33px #101010, -12px -12px 33px #1c1c1c;
		cursor: pointer;
	}
	.sponsors div p {
		font-size: 2rem;
	}
	.sponsors .sponsor3 img {
		margin-bottom: 40px;
	}
	.sponsors img {
		width: 200px;
	}
	.brouchure {
		position: fixed;
		inset: 50px;
		top: 80px;
		z-index: 100;
	}
	.brouchure embed {
		width: 90vw;
		height: 80vh;
	}
	.overlay {
		position: absolute;
		inset: 0;
		height: 100%;
		z-index: 100;
		width: 100%;
		background: rgba(0, 0, 0, 0.5);
	}
	.hidden {
		display: none;
	}
	.sponsors .sponsor {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.sponsors .sponsor p {
		margin-bottom: 50px;
	}
	@media (max-width: 900px) {
		.title {
			background-size: contain;
		}
		.title p {
			padding: 10px;
			font-size: 3rem;
		}

		.points {
			margin-top: 50px;
			width: 80vw;
		}
		.points ul li {
			font-size: 1.5rem;
		}

		.ending div {
			font-size: 1.5rem;
			margin: 1rem;
		}

		.our-sponsors {
			margin-top: 50px;
			height: auto;
		}
		.our-sponsors .sponsors {
			font-size: 1rem;
			margin: 0px;
			height: 80%;
		}
		.our-sponsors .sponsors div {
			align-self: center;
			margin: 1rem;
		}
		.sponsors div {
			padding: 20px;
			height: 200px;
		}
		.sponsors img {
			width: 100px;
		}
		.sponsors .sponsor3 img {
			margin-bottom: 20px;
		}
	}

	@media (max-width: 650px) {
		.title p {
			font-size: 2rem;
		}
		.points {
			margin: 50px auto;
		}
		.points ul li {
			font-size: 1rem;
		}
		.our-sponsors {
			height: auto;
		}
		.sponsors div {
			height: 150px;
			width: 70vw;
		}
		.sponsors img {
			width: 100px;
		}
		.sponsors div p {
			font-size: 1.5rem;
		}
	}
</style>
