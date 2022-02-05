<main>
	<h2>Competition</h2>
	<div class="numbers">
		<div class="blocks">
			50+ <br />
			<div class="labelBlock">Countries</div>
		</div>
		<div class="blocks">
			500+ <br />
			<div class="labelBlock">Teams</div>
		</div>
		<div class="blocks">
			10000+ <br />
			<div class="labelBlock">Students</div>
		</div>
	</div>
	<br /><br />
	<div class="comp">
		<p>
			Baja SAE challenges engineering students to design and build an off-road vehicle that will
			survive the severe punishment of rough terrain and in some competitions, water. As in real
			work situations, these future engineers work together as a team to discover and resolve
			technical challenges in design, test, and manufacturing, as well as business issues. The most
			rugged of all the competitions, Baja SAE also gives students the first-hand challenge of
			pursuing their passion while managing real-life demands and priorities. Each team's goal is to
			design and build a prototype of an all-weather, rugged, single-seat, off-road recreational
			vehicle intended for sale to the nonprofessional weekend off-road enthusiast
		</p>
		<br /><br />
	</div>
	<h3>
		The competition is divided into 2 categories - Static and Dynamics - which account for a total
		of 1000 points.
	</h3>
	<br /><br />
	<div class="events">
		<div class="eventBlocks">
			<div class="headEvents">STATIC EVENTS</div>
			<li>
				<ul class="blockElements">Design</ul>
				<ul class="blockElements">Cost Evaluation</ul>
				<ul class="blockElements">Sales Presentation</ul>
				<ul class="blockElements">Go Green</ul>
			</li>
		</div>
		<div class="eventBlocks">
			<div class="headEvents">DYNAMIC EVENTS</div>
			<li>
				<ul class="blockElements">Hill Climbs</ul>
				<ul class="blockElements">Sled Pulls</ul>
				<ul class="blockElements">Maneuverability Events</ul>
				<ul class="blockElements">Acceleration</ul>
				<ul class="blockElements">Rock crawls</ul>
				<ul class="blockElements">Suspension and traction Events</ul>
			</li>
		</div>
	</div>
	<div />
</main>

<style>
	main {
		display: grid;
		place-items: center;
		/**padding: 0.25rem 2rem;**/
	}
	h2 {
		background: url('./brushBg.png') center center;
		background-size: contain;
		font-weight: 4rem;
		font-size: 2rem;
		margin: 10px 0;
		font-family: url('./fonts/Chalkduster.ttf');
	}
	h3 {
		font-size: 2rem;
	}
	.numbers {
		background: url('./bg_comp.png');
		background-size: cover;
		background-repeat: no-repeat;
		width: 100%;
		background-attachment: scroll;
		display: flex;
		justify-content: space-evenly;
		align-items: center;
	}
	.blocks {
		font-size: 3rem;
		padding: 3rem;
	}
	.comp {
		padding: 2rem;
	}
	p {
		font-size: 1.5rem;
	}
	.labelBlock {
		font-size: 2rem;
	}
	.headEvents {
		background: url('./brushBg.png') center center;
		background-size: contain;
		justify-content: space-evenly;
		align-items: center;
		font-size: 2rem;
	}
	.events {
		display: flex;
		padding: 10%;
	}
	.eventBlocks {
		flex-direction: column;
		padding: 3rem;
		padding-left: 5rem;
		padding-right: 5rem;
	}
	.blockElements {
		font-size: 1.5rem;
	}
	@media (max-width: 720px) {
		.numbers {
			flex-direction: column;
		}
	}
</style>
