<script>
	import { onMount } from 'svelte';
	let checkBox;
	let links;
	onMount(() => {
		checkBox = document.getElementById('nav-check');
		links = document.querySelectorAll('.link');
		links.forEach((link) => {
			link.addEventListener('click', (e) => {
				console.log(window.location);
				links.forEach((link) => {
					link.classList.remove('active');
				});
				e.target.classList.add('active');
				if (checkBox.checked) {
					checkBox.checked = false;
				}
			});
		});
	});
</script>

<main>
	<nav>
		<div class="navbar">
			<div class="nav-header">
				<div class="nav-logo">
					<a href="/">
						<img src="./logo.png" width="100px" alt="Infinite Challengers Logo" />
					</a>
				</div>
			</div>

			<input type="checkbox" id="nav-check" />
			<div class="nav-btn">
				<label for="nav-check">
					<span />
					<span />
					<span />
				</label>
			</div>

			<div class="nav-links">
				<a href="/" class="link active">Home</a>
				<a href="/#about" class="link">About</a>
				<a href="/team" class="link">Team</a>
				<a href="/sponsers" class="link">Sponsers</a>
				<a href="/competition" class="link">Competition</a>
			</div>
		</div>
	</nav>
</main>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	nav {
		position: fixed;
		height: 80px;
		width: 100%;
		padding: 15px 40px;
		background-color: var(--primary-bg-color);
		z-index: 999;
	}
	.navbar .nav-header {
		display: inline;
	}
	.navbar .nav-header .nav-logo {
		display: inline-block;
		margin-top: -15px;
		margin-left: -25px;
	}
	.navbar .nav-links {
		display: inline;
		float: right;
		font-size: 18px;
		margin-top: 10px;
	}

	.nav-links a {
		position: relative;
	}

	.nav-links a:after {
		content: '';
		position: absolute;
		width: 100%;
		transform: scaleX(0);
		height: 2px;
		bottom: 0;
		left: 0;
		background-color: var(--primary-accent-color);
		transform-origin: bottom right;
		transition: transform 0.25s ease-out;
	}

	.nav-links a:hover:after {
		transform: scaleX(1);
		transform-origin: bottom left;
	}

	.navbar .nav-links a {
		margin: 10px 40px;
		text-decoration: none;
		font-weight: 550;
		color: white;
	}

	.navbar .nav-links .active {
		border-bottom: solid var(--primary-accent-color) 2px;
		transition: 0.3s ease;
	}
	.navbar .nav-links .active:hover {
		transform: none;
	}

	.navbar #nav-check,
	.navbar .nav-btn {
		display: none;
	}

	@media (max-width: 950px) {
		.navbar .nav-btn {
			display: inline-block;
			position: absolute;
			top: 0px;
			right: 0px;
		}
		.navbar .nav-btn label {
			display: inline-block;
			width: 80px;
			height: 70px;
			padding: 25px;
		}
		.navbar .nav-btn label span {
			display: block;
			height: 10px;
			width: 25px;
			border-top: 3px solid #eee;
		}

		.navbar .nav-links {
			position: absolute;
			display: block;
			text-align: center;
			width: 100%;
			background-color: var(--primary-bg-color);
			transition: all 0.3s ease-in;
			overflow-y: hidden;
			top: 70px;
			right: 0px;
		}
		.navbar .nav-links a {
			display: block;
		}
		.navbar .nav-links a:hover {
			color: var(--primary-accent-color);
		}
		.navbar .nav-links a::after {
			height: 0;
		}
		.navbar .nav-links .active {
			border: none;
			color: var(--primary-accent-color);
		}

		.navbar #nav-check:not(:checked) ~ .nav-links {
			height: 0px;
		}

		.navbar #nav-check:checked ~ .nav-links {
			height: calc(100vh - 70px);
			overflow-y: auto;
		}
	}
</style>
