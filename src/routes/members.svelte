<script>
	import { fade, fly, slide } from 'svelte/transition';
	import { onMount } from 'svelte';
	let ready = false;
	onMount(() => (ready = true));
</script>

<!-- ----------------------------------------------------------------- -->
<!-- ----------------------------------------------------------------- -->

<svelte:head>
	<title>infO(1)Robotics</title>
</svelte:head>

<main>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" />
	<link
		href="https://fonts.googleapis.com/css2?family=Orbitron&family=Roboto+Mono:wght@100&family=Share+Tech+Mono&display=swap"
		rel="stylesheet"
	/>
	<meta name="viewport" content="user-scalable=0;" />
	<div class="HTML">
		{#if ready}<nav in:fly={{ y: -50, duration: 500 }} class="nav" id="navbar">
				<a href="/3d">>3D View<span class="terminal">_</span></a>
				<a href="/members.html" class="nav-active">>Members<span class="terminal">_</span></a>
				<a href="/">>Home<span class="terminal">_</span></a>

				<a class="nav-logo" href="/">
					{#if ready}<img
							in:fade={{ duration: 2000 }}
							src="https://drive.google.com/uc?id=1eK_A6X-RjwRQrR1Ek0tPIGPCJonpFCB6"
							id="navbar-logo"
							alt="Logo"
						/>{/if}</a
				>
			</nav>{/if}
		<div id="main" />

		<link
			rel="stylesheet"
			href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"
		/>
		<input type="checkbox" id="active" />
		<label for="active" class="menu-btn"><i class="fas fa-bars" /></label>
		<div class="wrapper">
			<ul>
				<li><a href="/">Home</a></li>
				<li><a href="/members">Members</a></li>
				<li><a href="/3d">>3D View<span class="terminal">_</span></a></li>
			</ul>
		</div>
		{#if ready}<div in:fade={{ duration: 750 }}>
				{#if ready}<div in:fade={{ duration: 750 }} class="title">
						<h1>
							>Meet The <b>InfO(1)Robotics</b> Team<span class="terminal">_</span>
							<hr class="new6" />
						</h1>
					</div>{/if}
				{#if ready}<div in:fade={{ duration: 750 }} class="title2">
						<h1>
							>Team <b>Mentors</b><span class="terminal">_</span>
							<hr class="new5" />
						</h1>
					</div>{/if}
				{#if ready}<div in:fade={{ duration: 750 }} class="teammentors" style="top=0;">
						<div class="card_tudor">
							<img src="tudor.jpg" alt="Tudor Avram" style="width:100%" />
							<div class="container">
								<h2>>Tudor Avram<span class="terminal">_</span></h2>
								<p class="title1">>Team Mentor<span class="terminal">_</span></p>
							</div>
						</div>
						<div class="card">
							<img src="lica.jpg" alt="Dana Lica" style="width:100%" />
							<div class="container">
								<h2>>Daniela Lica<span class="terminal">_</span></h2>
								<p class="title1">>Team Mentor<span class="terminal">_</span></p>
							</div>
						</div>
						<div class="card1">
							<img src="soare.jpg" alt="Soare Stefan" style="width:100%" />
							<div class="container">
								<h2>>Stefan Soare<span class="terminal">_</span></h2>
								<p class="title1">>Technical Team Mentor<span class="terminal">_</span></p>
							</div>
						</div>
					</div>{/if}

				<!--TEMPLATE: 5:4 <div class="card" style="margin-right:0;">
            <img src="luminita.png" alt="Luminita Avram" style="width:100%">
            <div class="container">
              <h2>>Luminita Avram<span class="terminal">_</span></h2>
              <p class="title1">>Team Mentor<span class="terminal">_</span></p>
            </div>
        </div>
        </div> -->

				<div class="titlemobilefix">
					<div class="title4">
						<h1>
							>Team <b>Leaders</b><span class="terminal">_</span>
							<hr class="new5" />
						</h1>
					</div>
				</div>

				<div class="teamleaders">
					<div class="card1">
						<img src="sebi.jpg" alt="Sebastian Georgescu" style="width:100%" />
						<div class="container">
							<h2>>Sebastian Georgescu<span class="terminal">_</span></h2>
							<p class="title1">>Team Leader<span class="terminal">_</span></p>
						</div>
					</div>
					<div class="card">
						<img src="mada.jpg" alt="Madalina Andronache" style="width:100%" />
						<div class="container">
							<h2>>Madalina Andronache<span class="terminal">_</span></h2>
							<p class="title1">>PR Dept. Leader<span class="terminal">_</span></p>
						</div>
					</div>
					<div class="card2">
						<img src="alin.jpg" alt="Alin Andras" style="width:100%" />
						<div class="container">
							<h2>>Alin Andras<span class="terminal">_</span></h2>
							<p class="title1">>Technical Dept. Leader<span class="terminal">_</span></p>
						</div>
					</div>
					<div class="break" />
					<div class="card3">
						<img src="codrin.jpg" alt="Codrin Ristea" style="width:100%" />
						<div class="container">
							<h2>>Codrin Ristea<span class="terminal">_</span></h2>
							<p class="title1">>3D Design Dept. Leader<span class="terminal">_</span></p>
						</div>
					</div>

					<div class="card">
						<img src="alex.jpg" alt="Alexandru Sandulescu" style="width:100%" />
						<div class="container">
							<h2>>Alexandru Sandulescu<span class="terminal">_</span></h2>
							<p class="title1">>Programming Dept. Leader<span class="terminal">_</span></p>
						</div>
					</div>
				</div>
				<div class="title3">
					<h1>
						>Dept. <b>Members</b><span class="terminal">_</span>
						<hr class="new5" />
					</h1>
				</div>
				<div class="members">
					<div class="card1">
						<img src="alexandra.jpg" alt="Alexandra Popescu" style="width:100%" />
						<div class="container">
							<h2>>Alexandra Popescu<span class="terminal">_</span></h2>
							<p class="title1">
								>Technical Dept. Member - Assembly<span class="terminal">_</span>
							</p>
						</div>
					</div>

					<div class="card">
						<img src="anne.jpg" alt="Anne Biciin" style="width:100%" />
						<div class="container">
							<h2>>Anelisse Bîcîin<span class="terminal">_</span></h2>
							<p class="title1">
								>PR Dept. Member - Event Organiser<span class="terminal">_</span>
							</p>
						</div>
					</div>

					<div class="card_antonia">
						<img src="antonia.jpg" alt="Antonia Barbu" style="width:100%" />
						<div class="container">
							<h2>>Antonia Barbu<span class="terminal">_</span></h2>
							<p class="title1" style="font-size:15px;">
								>PR Dept. Member - Engineering Notebook<span class="terminal">_</span>
							</p>
						</div>
					</div>

					<div class="card_gabi">
						<img src="gabi.jpg" alt="Gabi Enache" style="width:100%" />
						<div class="container">
							<h2>>Gabi Enache<span class="terminal">_</span></h2>
							<p class="title1">
								>Technical Dept. Member - Assembly<span class="terminal">_</span>
							</p>
						</div>
					</div>
					<div class="card1">
						<img src="mihai.jpg" alt="plex" style="width:100%" />
						<div class="container">
							<h2>>Mihail Cimpoiasu<span class="terminal">_</span></h2>
							<p class="title1">
								>Technical Dept. Member - Programmer<span class="terminal">_</span>
							</p>
						</div>
					</div>

					<div class="card1">
						<img src="rares.jpg" alt="Rares Neagoe" style="width:100%" />
						<div class="container">
							<h2>>Rares Neagoe<span class="terminal">_</span></h2>
							<p class="title1">>PR Dept. Member - Social Media<span class="terminal">_</span></p>
						</div>
					</div>
					<div class="card1">
						<img src="cretu.jpg" alt="Sebastian Cretu" style="width:100%" />
						<div class="container">
							<h2>>Sebastian Cretu<span class="terminal">_</span></h2>
							<p class="title1">
								>Technical Dept. Member - 3D Design<span class="terminal">_</span>
							</p>
						</div>
					</div>

					<div class="card">
						<img src="vlad.jpg" alt="Vlad Dinu" style="width:100%" />
						<div class="container">
							<h2>>Vlad Dinu<span class="terminal">_</span></h2>
							<p class="title1">
								>Technical Dept. Member - Assembly<span class="terminal">_</span>
							</p>
						</div>
					</div>
				</div>

				<div class="logosection">
					<a href="http://www.cn-caragiale.ro/"
						><img
							src="https://drive.google.com/uc?id=1qmTs5j8PyzxNZhE41bgmG_tiLSgFzrJN"
							alt="INSTAGRAM"
						/></a
					>
					<a href="https://natieprineducatie.ro/"
						><img
							src="https://drive.google.com/uc?id=1wl1WxYU-KNe5f72ATPCTDAzOvBTiDq31"
							alt="FTC"
							style="margin-left:1%;"
						/></a
					>
					<a href="https://www.instagram.com/info1robotics/"
						><img
							src="https://drive.google.com/uc?id=1hGjq4VzAa9Xrz8v5uSjvWk1T2qNpZkPn"
							alt="INSTAGRAM"
						/></a
					>
				</div>
				<div class="linkssection">
					<a href="https://www.instagram.com/info1robotics/"
						><img
							src="https://drive.google.com/uc?id=1cMI5UrBOrvltwZ090ys5m7wCe4c1u4fd"
							alt="INSTAGRAM"
						/></a
					>
					<a href="https://www.facebook.com/info1robotics/"
						><img
							src="https://drive.google.com/uc?id=1YDEBin_npoElopwus2CouhVJqNORE8aM"
							alt="FACEBOOK"
						/></a
					>
					<a href="https://www.youtube.com/channel/UC6PkNCRNEQOfKuciVltqzTQ"
						><img
							src="https://drive.google.com/uc?id=1HndKVFjySGNx1edEEH9OXP7zRnRA4qUG"
							alt="YOUTUBE"
						/></a
					>
					<a href="https://open.spotify.com/show/6glFbyo8OnIqih7RuPjB1e"
						><img
							src="https://drive.google.com/uc?id=1ki_ydOgY3Kz7qzI3m12DP1EgLvndMa6B"
							alt="SPOTIFY"
						/></a
					>
					<a href="mailto: info1robotics@gmail.com"
						><img
							src="https://drive.google.com/uc?id=17d8EWjB6gFm1NVgigRpdm1iHloEFQDIk"
							alt="EMAIL"
						/></a
					>
				</div>
			</div>{/if}
	</div>
</main>

<!-- ----------------------------------------------------------------- -->
<style>
	:global(body) {
		scroll-behavior: smooth;
		margin: 0;
		padding: 0;
		background-color: #15181e;
		background-repeat: no-repeat;
		background-size: cover;
		background-position: center;
		font-family: 'orbitron';
		overflow-x: hidden;
		margin: 0;
		padding: 0;
	}
	.nav {
		position: relative;
		top: 0;
		z-index: 100;
		padding-left: 4vh;
		padding-right: 4vh;
		height: 7vh;
		background-color: #15181e;
		box-sizing: border-box;
		position: fixed;
		width: 100%;
		transition: all 0.3s ease-in-out;
	}
	.nav a {
		padding: 2.5vh 2.8vh 2.6vh 1.2vh;
		float: right;
		text-transform: uppercase;
		font-size: 1.7vh;
		font-weight: 500;
		text-decoration: none;
		color: #fff;
		transition: all 0.2s ease-in-out;
	}

	.nav > .nav-logo {
		padding: 1vh 0 3vh 5vh;
		float: left;
		position: relative;
		left: 5vh;
	}
	.nav-logo img {
		height: 5vh;
		margin: 0;
		transition: all 0.3s ease-in-out;
	}
	img:hover {
		transform: rotate(360deg);
	}
	.nav a {
		font-size: 1.5vh;
	}
	.nav a:hover {
		transform: scale(1.2);
	}
	.nav > .nav-active {
		color: #39b44a;
	}
	@media only screen and (max-width: 1000px) {
		.nav {
			display: none;
		}
	}
	.nav a {
		float: center;
		font-size: 1.3vh;
	}
	@import url('https://fonts.googleapis.com/css?family=Poppins:400,500,600,700&display=swap');
	.wrapper {
		z-index: 200;
		position: fixed;
		top: 0;
		left: 0;
		height: 100%;
		width: 100%;
		background: linear-gradient(#39b44a, #0b6623);
		clip-path: circle(25px at calc(100% - 60px) 4.5vh);
		transition: all 0.3s ease-in-out;
	}
	#active:checked ~ .wrapper {
		clip-path: circle(75%);
	}
	.menu-btn {
		position: fixed;
		z-index: 201;
		right: 1.4vh;
		top: 2vh;
		height: 5vh;
		width: 5vh;
		text-align: center;
		line-height: 5vh;
		border-radius: 50%;
		font-size: 2vh;
		color: #fff;
		cursor: pointer;
		background: #15181e;
		transition: all 0.3s ease-in-out;
	}
	#active:checked ~ .menu-btn {
		background: #fff;
		color: #39b44a;
	}
	#active:checked ~ .menu-btn i:before {
		content: '\f00d';
	}
	.wrapper ul {
		position: relative;
		top: 50%;
		list-style: none;
		text-align: center;
	}
	.wrapper ul li {
		margin: 15px 0;
	}
	.wrapper ul li a {
		color: none;
		text-decoration: none;
		font-size: 4vh;
		font-weight: 500;
		padding: 5px 30px;
		color: #fff;
		position: relative;
		line-height: 5vh;
		transition: all 0.3s ease;
	}
	.wrapper ul li a:after {
		position: absolute;
		content: '';
		background: #000;
		width: 100%;
		height: 100px;
		left: 0;
		border-radius: 50px;
		transform: scaleY(0);
		z-index: -1;
		transition: transform 0.3s ease;
	}
	.wrapper ul li a:hover:after {
		transform: scaleY(1);
	}
	.wrapper ul li a:hover {
		color: #fff;
	}
	input[type='checkbox'] {
		display: none;
	}
	@media (min-width: 60vh) {
		.wrapper {
			display: none;
		}
		.menu-btn {
			display: none;
		}
	}
	hr.new5 {
		border: 3px solid #d0d3e1;
		border-radius: 3px;
		width: 21.5%;
	}
	hr.new6 {
		border: 3px solid #d0d3e1;
		border-radius: 3px;
		width: 38.5%;
	}
	@media only screen and (max-width: 1000px) {
		hr.new5 {
			width: 32vw;
		}
		hr.new6 {
			width: 60%;
		}
	}
	.title {
		position: relative;
		top: 10vh;
	}
	.title2 {
		position: relative;
		top: 14vh;
	}
	.title3 {
		position: relative;
		top: -3.5vh;
	}
	.title4 {
		position: relative;
		top: 14vh;
	}
	@media only screen and (max-width: 1000px) {
		.title {
			top: 5vh;
		}
		.title2 {
			top: 12vh;
		}
		.title3 {
			top: -1vh;
		}
		.title4 {
			top: 6vh;
		}
	}
	h1 {
		color: #d0d3e1;
		text-align: center;
	}
	b {
		color: #39b44a;
	}

	.terminal {
		animation: blink 1s infinite step-end;
	}
	@keyframes blink {
		from,
		to {
			opacity: 0;
		}
		50% {
			opacity: 1;
		}
	}

	*,
	*:before,
	*:after {
		box-sizing: inherit;
	}

	.card {
		box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
		background-color: #d0d3e1;
		border-radius: 25px;
		position: relative;
		height: 400px;
		width: 400px;
		display: table;
		flex: 0 0 auto;
		height: 50px;
		border: 1px solid black;
		margin-right: 1.5%;
		margin-left: 1.5%;
		margin-bottom: 3%;
	}
	.card1 {
		box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
		background-color: #d0d3e1;
		border-radius: 25px;
		position: relative;
		height: 400px;
		width: 400px;
		display: table;
		flex: 0 0 auto;
		height: 50px;
		border: 1px solid black;
		margin-right: 1.5%;
		margin-left: 1.5%;
		margin-bottom: 3%;
	}
	.card_tudor {
		box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
		background-color: #d0d3e1;
		border-radius: 25px;
		position: relative;
		height: 400px;
		width: 400px;
		display: table;
		flex: 0 0 auto;
		height: 50px;
		border: 1px solid black;
		margin-right: 1.5%;
		margin-left: 1.5%;
		margin-bottom: 3%;
	}
	.card_antonia {
		box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
		background-color: #d0d3e1;
		border-radius: 25px;
		position: relative;
		height: 400px;
		width: 400px;
		display: table;
		flex: 0 0 auto;
		height: 50px;
		border: 1px solid black;
		margin-right: 0;
		margin-right: 1.5%;
		margin-left: 1.5%;
		margin-bottom: 3%;
	}
	.card_gabi {
		box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
		background-color: #d0d3e1;
		border-radius: 25px;
		position: relative;
		height: 400px;
		width: 400px;
		display: table;
		flex: 0 0 auto;
		height: 50px;
		border: 1px solid black;
		margin-bottom: 3%;
		margin-right: 1.5%;
		margin-left: 1.5%;
	}
	@media only screen and (max-width: 1000px) {
		.card_antonia {
			margin-right: 3%;
		}
		.card_gabi {
			margin-left: 5%;
			margin-right: 0;
		}
		.card_tudor {
			margin-left: 0;
		}
	}
	.card2 {
		box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
		background-color: #d0d3e1;
		border-radius: 25px;
		position: relative;
		height: 400px;
		width: 400px;
		display: table;
		flex: 0 0 auto;
		height: 50px;
		border: 1px solid black;
		margin-right: 1.5%;
		margin-left: 1.5%;
		margin-bottom: 3%;
	}
	.card3 {
		box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
		background-color: #d0d3e1;
		border-radius: 25px;
		position: relative;
		height: 400px;
		width: 400px;
		display: table;
		flex: 0 0 auto;
		height: 50px;
		border: 1px solid black;
		margin-right: 1.5%;
		margin-left: 1.5%;
		margin-bottom: 3%;
	}
	@media only screen and (max-width: 1000px) {
		.card1 {
			margin-right: 3%;
		}

		.card {
			margin-right: 0;
		}

		.card3 {
			margin-right: 0;
		}
		.card3 {
			margin-left: 3%;
		}
	}
	.break {
		flex-basis: 100%;
		height: 0;
	}
	@media only screen and (max-width: 1000px) {
		.break {
			flex-basis: 0%;
		}
	}
	.card img {
		border-top-left-radius: 25px;
		border-top-right-radius: 25px;
	}
	.card1 img {
		border-top-left-radius: 25px;
		border-top-right-radius: 25px;
	}
	.card_tudor img {
		border-top-left-radius: 25px;
		border-top-right-radius: 25px;
	}
	.card_antonia img {
		border-top-left-radius: 25px;
		border-top-right-radius: 25px;
	}
	.card_gabi img {
		border-top-left-radius: 25px;
		border-top-right-radius: 25px;
	}
	.card2 img {
		border-top-left-radius: 25px;
		border-top-right-radius: 25px;
	}
	.card3 img {
		border-top-left-radius: 25px;
		border-top-right-radius: 25px;
	}
	.container {
		padding: 0 16px;
	}
	.title1 {
		color: grey;
	}
	.teamleaders {
		position: relative;
		margin-top: 20vh;
		display: flex;
		flex-wrap: wrap;
		align-items: center;
		justify-content: center;
	}
	@media only screen and (max-width: 1000px) {
		.titlemobilefix {
			margin-top: 7vh;
		}
		.teamleaders {
			margin-top: 8vh;
		}
	}
	.members {
		position: relative;
		display: flex;
		flex-wrap: wrap;
		align-items: center;
		justify-content: center;
	}
	.linkssection {
		position: relative;
		top: 15vh;
	}
	.linkssection img {
		position: relative;
		width: 19.5vw;
		height: auto;
	}
	.logosection {
		position: relative;
		top: 10vh;
	}
	.logosection img {
		height: auto;
		width: 32vw;
	}
	@media only screen and (max-width: 1000px) {
		.linkssection {
			top: 10vh;
		}
	}
	@media only screen and (max-width: 1000px) {
		.logosection {
			top: 5vh;
		}
	}
	.teammentors {
		position: relative;
		top: 17vh;
		display: flex;
		flex-wrap: wrap;
		align-items: center;
		justify-content: center;
	}
	@media only screen and (max-width: 1000px) {
		.teammentors {
			top: 13vh;
		}
	}
</style>
