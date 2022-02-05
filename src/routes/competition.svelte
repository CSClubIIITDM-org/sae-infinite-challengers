<script>
	import Saos from 'saos';
</script>

<main>
	<Saos animation={'from-bottom 1s cubic-bezier(0.35, 0.5, 0.65, 0.95)'}>
	<div class="about-us__stats">
        <div class="about-us__stats1">
            <h1><b>50+</b></h1>
            <p>Countries</p>
        </div>
        <div class="about-us__stats2">
            <h1><b>500+</b></h1>
            <p>Teams</p>
        </div>
        <div class="about-us__stats3">
            <h1><b>10000+</b></h1>
            <p>Students</p>
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
	</Saos>
</main>

<style>
	main {
		display: grid;
		place-items: center;
		width: 100vw !important;
		overflow-y: hidden;
	}
	
	h3 {
		text-align: center;
		font-size: 2rem;
	}

	.about-us__stats {
		width: 100vw;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-evenly;
        align-items: center;
        margin: 7rem 0 2rem 0;
        height: 350px;
        background: linear-gradient(rgba(0, 0, 0, 0.67), rgba(0, 0, 0, 0.67)), url('/static/bg_comp.png') center center no-repeat;
		background-size: cover;
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
	
	.comp {
		padding: 0 2rem;
	}
	.comp p {
		text-align: center;
		font-size: 1.5rem;
	}
	h3 {
		font-size: 1.5rem;
		padding: 0 2rem;
	}
	.headEvents {
		font-style: italic;
		font-weight: bold;
		color: var(--primary-accent-color);
		justify-content: space-evenly;
		align-items: center;
		font-size: 2rem;
		margin: 2rem 0;
	}
	.events {
		width: 60vw;
		display: flex;
		justify-content: space-around;
		margin: 0 auto 50px auto;
	}
	.eventBlocks {
		flex-direction: column;
		padding: 3rem;
	}
	.blockElements {
		font-size: 1.5rem;
	}
	
</style>
