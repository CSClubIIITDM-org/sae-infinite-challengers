<footer>
	<h1 class="heading">Contact Us</h1>
	<div class="flex-container location_info">
		<div class="flex-item-left">
			<div class="address">
				<h3>Infinite Challengers</h3>
				<p>IIITDM Kancheepuram Campus, Chennai, TamilNadu-600127</p>
				<p>Email:saeclub@iiitdm.ac.in</p>

				<br />

				<h3>Vineet Sengar</h3>
				<p>Team Captain</p>
				<p>Mob No:+91 91316 93095</p>
				<p>Email: mpd17i018@iiitdm.ac.in</p>

				<br />

				<h3>Mitelesh</h3>
				<p>Team Captain</p>
				<p>Mob No:+91 91766 77701</p>
				<p>Email: mpd18i008@iiitdm.ac.in</p>

				<br />

				<h3>Sukesh</h3>
				<p>Team Manager</p>
				<p>Mob No:+91 86103 81270</p>
				<p>Email: mdm19b024@iiitdm.ac.in</p>

				<br />

				<br />
				<br />
			</div>
		</div>
		<div class="flex-item-right">
			<a href="https://goo.gl/maps/NZBSQfC8KD9aRJFr5">
				<img src="./institute-map.png" alt="Institute map" />
				<div class="overlay">
					<img src="./sponsors/iiitdm.svg" alt="IIITDM-Logo" />
				</div>
			</a>
		</div>
	</div>
	<h2 class="copyright">Developed by <span>CS Club</span></h2>
</footer>

<style>
	* {
		box-sizing: border-box;
		scroll-behavior: smooth;
	}
	.location_info {
		margin-top: 45px;
	}
	.heading {
		font-family: var(--primary-font);
		font-style: italic;
		color: var(--primary-accent-color);
		font-size: 4rem;
		text-align: center;
		font-weight: bolder;
	}
	h3 {
		color: var(--primary-accent-color);
	}

	h2 span {
		color: var(--primary-accent-color);
	}
	.flex-container {
		display: flex;
		flex-direction: row;
		text-align: left;
	}

	.flex-item-left {
		padding-left: 20px;
		flex: 50%;
		font-size: 18px;
	}

	.flex-item-right {
		padding: 10px;
		flex: 50%;
		display: grid;
		/* position: relative; */
		place-items: center;
	}
	.flex-item-right a {
		position: relative;
	}
	.flex-item-right img {
		width: 600px;
		height: 500px;
		border-radius: 10px;
	}

	.copyright {
		text-align: center;
		font-size: 25px;
	}

	.overlay {
		position: absolute;
		inset: 0;
		height: 100%;
		width: 100%;
		background: rgba(0, 0, 0, 0.5);
		display: flex;
		align-items: center;
	}

	.overlay img {
		height: 50%;
	}
	@media (max-width: 950px) {
		.location_info {
			margin-top: 20px;
		}
		.flex-container {
			flex-direction: column;
			text-align: center;
		}
		.flex-item-left {
			font-size: 15px;
		}
		.flex-item-right img {
			width: 270px;
			height: 225px;
			border-radius: 10px;
		}
		.heading {
			font-size: 3rem;
			margin-top: 15px;
		}
		.copyright {
			font-size: 15px;
		}
	}

	@media (max-width: 720px) {
		.location_info {
			margin-top: 10px;
		}
		.flex-container {
			flex-direction: column;
			text-align: center;
		}
		.flex-item-left {
			font-size: 13px;
		}
		.flex-item-right img {
			width: 240px;
			height: 180px;
			border-radius: 10px;
		}
		.heading {
			font-size: 2rem;
			margin-top: 15px;
		}
		.copyright {
			font-size: 13px;
		}
	}
</style>
