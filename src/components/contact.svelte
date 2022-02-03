<footer class="contact">
	<h1 class="heading">Contact Us</h1>
	<section class="location-info row">
		<div class="address column">
			<div>
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

				<h2>Developed by <span>CS Club</span></h2>

				<br />
				<br />
			</div>
		</div>
		<div class="map column">
			<a href="https://goo.gl/maps/NZBSQfC8KD9aRJFr5">
				<img src="/static/institute-map.png" alt="Institute map" />
			</a>
		</div>
	</section>
</footer>

<style>
	.location-info {
		margin-top: 45px;
	}
	.heading {
		font-family: var(--secondary-font);
	}
	h1 {
		background: url('./brushBg.png') no-repeat center center;
		font-weight: bolder;
		margin: 10px 600px 10px 500px;
		background-size: 425px 100px;
		font-size: 60px;
	}
	h3 {
		color: var(--primary-accent-color);
	}

	h2 span {
		color: var(--primary-accent-color);
	}

	.column {
		float: left;
		width: 45%;
	}

	.row:after {
		content: '';
		display: table;
		clear: both;
	}
	.address {
		padding-left: 40px;
	}

	.address p {
		font-size: 18px;
	}

	.map img {
		width: 600px;
		height: 500px;
		padding-left: 25px;
	}

	@media screen and (max-width: 720px) {
		.heading {
			width: 25%;
			font-size: 30px;
			padding: 0;
			margin: 0 0 0 250px;
			background: url('./brushBg.png') no-repeat center center;
			background-size: contain;
		}
		.address {
			width: 70%;
		}
		.map {
			width: 100%;
		}
		.map img {
			width: 80%;
		}
	}
</style>
