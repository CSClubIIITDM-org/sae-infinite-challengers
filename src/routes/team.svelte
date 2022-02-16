<script>
	import teams from './../../static/teams/teams-data.json';
	import Saos from 'saos';
</script>

<main>
	<h1 class="heading">Team</h1>
	{#each teams as team (team.id)}
		<Saos animation={'from-bottom 1s cubic-bezier(0.35, 0.5, 0.65, 0.95)'} once={true}>
			<section>
				<div class="title">
					<h1>{team.id}</h1>
					<h2>{team.title}</h2>
				</div>
				<div class="members" class:mem3={team.members.length === 3}>
					{#each team.members as member}
						<div class="member" class:lead={member.id == 1}>
							<img src="./teams/{team.title}/{member.id}.png" alt="member-img" />
							<div class="member-details">
								<h1>{member.role}</h1>
								<h2>{member.name}</h2>
							</div>
						</div>
					{/each}
				</div>
			</section>
		</Saos>
	{/each}
</main>

<style>
	main {
		width: 80vw;
		margin: auto auto;
		padding-top: 10px;
	}
	.heading {
		margin-top: 100px;
		font-family: var(--primary-font);
		font-style: italic;
		font-size: 4rem;
		font-weight: bold;
		color: var(--primary-accent-color);
		text-align: center;
	}
	.title {
		margin: 1rem 0;
		position: relative;
		height: 5rem;
	}
	.title::before {
		content: '';
		position: absolute;
		bottom: 0;
		left: -20px;
		width: 8px;
		height: 80%;
		background: var(--primary-accent-color);
	}
	.title h1 {
		position: absolute;
		font-size: 4rem;
		color: var(--secondary-trans-text-color);
		inset: 0;
	}
	.title h2 {
		position: absolute;
		font-size: 2rem;
		bottom: 0;
		left: 40px;
		text-transform: uppercase;
	}
	.members {
		display: grid;
		width: 100%;
		grid-template-columns: 33.33% 33.33% 33.33%;
		gap: 10px;
		margin: 50px 0;
	}
	.members.mem3 {
		grid-template-columns: 50% 50%;
	}
	.member {
		margin: 30px 0;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		width: 100%;
	}
	.member img {
		height: 200px;
		-webkit-box-reflect: below 0 linear-gradient(transparent, transparent, rgba(0, 0, 0, 0.1));
	}
	.member-details {
		margin-top: 20px;
		position: relative;
		width: 100%;
		height: 3.5rem;
	}
	.member-details h1 {
		position: absolute;
		font-size: 1.3rem;
		left: 50%;
		transform: translate(-50%);
		color: var(--secondary-trans-text-color);
		top: 0;
		text-transform: uppercase;
	}
	.member-details h2 {
		position: absolute;
		font-size: 1.35rem;
		left: 50%;
		transform: translate(-50%);
		bottom: 0;
	}
	.lead {
		grid-column: 1/4;
	}
	@media (max-width: 768px) {
		.members {
			margin: 10px 0;
		}
		main {
			width: 95vw;
			overflow-x: hidden;
		}
		.member {
			margin: 10px 0;
		}
		.member img {
			height: 100px;
		}
		.member-details {
			margin-top: 10px;
			height: 2rem;
		}
		.member-details h1 {
			font-size: 0.7rem;
		}
		.member-details h2 {
			font-size: 0.7rem;
		}
		.title {
			height: 3rem;
		}
		.title::before {
			content: '';
			position: absolute;
			bottom: 0;
			left: -50px;
			width: 8px;
			height: 80%;
			background: var(--primary-accent-color);
		}
		.title h1 {
			font-size: 2rem;
		}
		.title h2 {
			font-size: 1rem;
		}
	}
	@keyframes -global-from-bottom {
		0% {
			opacity: 0;
			transform: translateY(50vw);
		}
		50% {
			opacity: 0.5;
		}
		100% {
			opacity: 1;
			transform: translateX(0);
		}
	}
</style>
