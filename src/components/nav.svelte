<script>
	function handleClick() {
		var links = document.querySelectorAll('.link');
		Array.from(links).forEach((item) => {
			item.addEventListener('click', () => {
				var selected = document.getElementsByClassName('active');
				selected[0].className = selected[0].className.replace(' active', '');
				item.className += ' active';
			});
		});
	}
</script>

<main>
	<div class="navbar">
		<div class="nav-header">
			<div class="nav-logo">
				<a href="/">
					<img src="/static/logo.png" width="100px" alt="Infinite Challengers Logo" />
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

		<div class="nav-links" on:click={handleClick}>
			<a href="/" class="link active">Home</a>
			<a href="/#about" class="link">About</a>
			<a href="/team" class="link">Team</a>
			<a href="/sponsers" class="link">Sponsers</a>
			<a href="/competition" class="link">Competition</a>
		</div>
	</div>
</main>

<style>
	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	.navbar {
		height: 100px;
		width: 100%;
		padding: 15px 40px;
		position: relative;
	}
	.navbar .nav-header {
		display: inline;
	}
	.navbar .nav-header .nav-logo {
		display: inline-block;
		margin-top: -19px;
		margin-left: -30px;
	}
	.navbar .nav-links {
		display: inline;
		float: right;
		font-size: 18px;
		margin-top: 10px;
	}
	.active {
		background: url('./static/brushBg.png') no-repeat center center;
		background-size: contain;
		border-radius: 5px;
		transition: 0.3s ease;
	}
	.navbar .nav-links a {
		padding: 10px 40px 10px;
		text-decoration: none;
		font-weight: 550;
		color: white;
	}
	.navbar .nav-links a:hover {
		background: url('./brushBg.png') no-repeat center center;
		background-size: contain;
	}

	.navbar #nav-check,
	.navbar .nav-btn {
		display: none;
	}

	@media (max-width: 720px) {
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
			background-color: black;
			transition: all 0.3s ease-in;
			overflow-y: hidden;
			top: 70px;
			right: 0px;
		}
		.navbar .nav-links a {
			display: block;
		}
		.navbar .nav-links a:hover {
			background: url('./brushBg.png') center center;
			background-size: cover;
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
