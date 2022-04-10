<script>
	import { fade, fly, slide } from 'svelte/transition'; // Svelte - Transitions
	import { onMount } from 'svelte'; // Svelte - JS Load
	// import Particles from 'svelte-particles'; // Background Typescript-Based tsParticles Library
	// import { inview } from 'svelte-inview/src';
	// let isInView;
	let ready = false;
	onMount(() => (ready = true));
</script>

<svelte:head>
	<title>infO(1)Robotics</title>
</svelte:head>

<html lang="en">
	<!-- Fonts Loader - Google API -->

	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" />
	<link
		href="https://fonts.googleapis.com/css2?family=Orbitron&family=Roboto+Mono:wght@100&family=Share+Tech+Mono&display=swap"
		rel="stylesheet"
	/>
	<meta name="viewport" content="user-scalable=0;" />

	<div class="HTML" />

	<!-- Desktop Navigation Bar -->

	{#if ready}<nav in:fly={{ y: -50, duration: 500 }} class="nav" id="navbar">
			<a href="/3D">>3D Renders<span class="terminal">_</span></a>
			<a href="/members">>Members<span class="terminal">_</span></a>
			<a href="/" class="nav-active">>Home<span class="terminal">_</span></a>

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

	<!-- Mobile Navigation Menu -->

	<link
		rel="stylesheet"
		href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"
	/>
	<input type="checkbox" id="active" />
	<label for="active" class="menu-btn"><i class="fas fa-bars" /></label>

	<div class="wrapper">
		<ul>
			<li><a href="/">>Home<span class="terminal">_</span></a></li>
			<li>
				<a href="/members">>Members<span class="terminal">_</span></a>
			</li>
			<li><a href="/3d">>3D Renders<span class="terminal">_</span></a></li>
		</ul>
	</div>

	<!-- Splash Screen -->

	<div class="splashscreen">
		<!-- Ongoing issue: the background particles are fixed to the screen -->

		<span class="splash-title">
			{#if ready}<h1 in:fly={{ x: -2000, duration: 1000 }}>inf<b>O(1)</b></h1>{/if}
			{#if ready}<h1 in:fly={{ x: -2000, duration: 1100 }}>Robotics</h1>{/if}
			{#if ready}<p in:fly={{ x: -2000, duration: 1250 }}>
					>Aspire to <b>INSPIRE</b>💚<span class="terminal">_</span>
				</p>{/if}
		</span>
		{#if ready}<div class="alignCAD">
				<img src="robot.png" alt="CAD" in:fly={{ x: 2000, duration: 1250 }} />
			</div>{/if}
			{#if ready}<div in:fly={{ x: 2000, duration: 1000 }} class="spinning"><img src="vortex.svg" alt="vortex"/></div>{/if}
		</div>

	<!-- About Us Section -->

	<!-- <div 	
use:inview={{ unobserveOnEnter: true, rootMargin: '-20%' }}
on:change={({ detail }) => {
isInView = detail.inView;
}}
>
FOR FUTURE USE
</div> -->

	<div class="aboutus">
		{#if ready}<h1 in:fade={{ duration: 2000 }} style="margin-top:2.5%;">
				>We are Inf<b>O(1)</b> Robotics<span class="terminal">_</span>
			</h1>{/if}
		{#if ready}<p in:fade={{ duration: 2000 }}>
				><b>We</b> are the <b>infO(1)Robotics</b> Team – RO 140 - from “Ion Luca Caragiale” High
				School from Ploiesti, Romania. Our team started out in April 2018, and it is coordinated by
				our mentors <b> Daniela Lica</b>, a Computer Science teacher, and <b> Tudor Avram</b>, a
				Software Engineer and our Technical mentor, <b> Stefan Soare</b>, a UVT student<span
					class="terminal">_</span
				>
			</p>{/if}
		{#if ready}<img
				in:fade={{ duration: 2000 }}
				src="podium.png"
				alt="ok"
				style="width:60%;"
			/>{/if}
		{#if ready}<p in:fade={{ duration: 2000 }}>
				><b>Our team</b> is composed of 15 members and over 50 volunteers and each of them is
				currently working in the STEM fields with extracurricular activities which fit their
				sub-teams.
				<b>We</b> started out with no budget and has been gradually building up our financial
				resources<span class="terminal">_</span>
			</p>{/if}
		{#if ready}<img
				in:fade={{ duration: 2000 }}
				src="robot0.png"
				alt="ok"
				style="width:50%;"
			/>{/if}
		{#if ready}<p in:fade={{ duration: 2000 }}>
				><b>infO(1)Robotics</b> is currently participating in the <b>FIRST Tech Challenge</b> high
				school robotics competition and expects to develop a greater knowledge for the future’s main
				goal: <b>Robots</b> and <b>Artificial Intelligence</b><span class="terminal">_</span>
			</p>{/if}
		{#if ready}<img
				in:fade={{ duration: 2000 }}
				src="vladrandom.png"
				alt="ok"
				style="width:50%;"
			/>{/if}
		{#if ready}<p in:fade={{ duration: 2000 }}>
				><b>We</b> combine work and pleasure, we <b>as a team</b>
				always train hard but in an enjoyable way. By sharing opinions and learning about team work,
				we believe we can get creative enough to someday find a revolutionary and feasible idea of a
				robot that could unbelievably help humanity in its own way<span class="terminal">_</span>
			</p>{/if}

		{#if ready}<h1 in:fade={{ duration: 2000 }} style="margin-top:2.5%;">
				>We are constantly <b>evolving</b><span class="terminal">_</span>
			</h1>{/if}
		{#if ready}<h1 in:fade={{ duration: 2000 }} style="margin-top:2.5%;">
				>2018-2019<span class="terminal">_</span>
			</h1>{/if}

		{#if ready}<p in:fade={{ duration: 2000 }}>
				><b>Inf0(1) Robotics</b> estabilished in late octomber and, <b>as rookies</b>, we faced a
				lot of problems. Despite our first year, we won the Bucharest Regional as 2nd pick and at
				the National Stage, we won <b>Inspire 3</b><span class="terminal">_</span>
			</p>{/if}
		{#if ready}<img in:fade={{ duration: 2000 }} src="2018.png" alt="ok" style="width:50%;" />{/if}

		{#if ready}<h1 in:fade={{ duration: 2000 }} style="margin-top:2.5%;">
				>2019-2020<span class="terminal">_</span>
			</h1>{/if}

		{#if ready}<p in:fade={{ duration: 2000 }}>
				>During the Skystone season, <b>Inf0(1) Robotics</b> created numerous events (e.g. Inf0(1)
				Talks, Inf0(1) Demo, etc.) and won a great deal of demos (e.g. Qube Demo, RobotX Demo etc.).
				When the pandemic started, we decided to create plastic face-shields for medical staff in
				need. We donated a total of <b>2401 face-shields</b> to <b>32 institutions</b>. Inf0(1)
				Robotics won <b>Inspire 1</b> at Bucharest Regional<span class="terminal">_</span>
			</p>{/if}

		{#if ready}<img
				in:fade={{ duration: 2000 }}
				src="spital.jpg"
				alt="ok"
				style="width:50%;"
			/>{/if}
		{#if ready}<p
				in:fade={{ duration: 2000 }}
				style="margin-left:30vw;margin-right:30vw;margin-top:2.5vh;font-size:75%;"
			>
				Letter from the <b>Ploiesti Pedriatic Hospital</b>: <b>infO(1)Robotics</b> is "contaminated"
				with
				<b>a spirit of sacrifice and dedication for the greater good</b> of the local community<span
					class="terminal">_</span
				>
			</p>{/if}

		{#if ready}<h1 in:fade={{ duration: 2000 }} style="margin-top:2.5%;">
				>2020-2021<span class="terminal">_</span>
			</h1>{/if}

		{#if ready}<p in:fade={{ duration: 2000 }}>
				>As the pandemic continued, <b>Ultimate Goal</b> has been a <b>challenging season</b> where
				demos and events were held <b>remotely</b>. In that season we created <b>Po(1)cast</b> where
				we invited a lot of teams and members from the <b>FTC community</b>. At the Bucharest
				Regional, <b>Inf0(1) Robotics</b> won Control Award for its robot great autonomous period<span
					class="terminal">_</span
				>
			</p>{/if}

		{#if ready}<img in:fade={{ duration: 2000 }} src="2020.png" alt="ok" style="width:50%;" />{/if}

		{#if ready}<h1 in:fade={{ duration: 2000 }} style="margin-top:2.5%;">
				>2021-2022<span class="terminal">_</span>
			</h1>{/if}

		{#if ready}<p in:fade={{ duration: 2000 }}>
				>So far, in the <b>2021-2022</b> FTC Freight Frenzy Season we won multiple awards, such as
				<b>1st place</b>
				and Design Award at the <b>Russian FTC Remote Regional</b>, <b>1st place</b>
				and <b>Inspire 2nd</b> at the #3 FTC Romania Iasi & Bucharest Regional, <b>Inspire 1st</b>
				at the <b>Romania National Championship</b> and we are looking forward in participating at
				the
				<b>FTC 2022 World Championship</b>. Besides building robots, we organized multiple
				<b>educational events</b>, such as the <b>AFI Ploiesti STEM Week</b> and charitable events
				for children in need and <b>Ukrainian refugees</b>💚<span class="terminal">_</span>
			</p>{/if}

		{#if ready}<img in:fade={{ duration: 2000 }} src="poppy.png" alt="ok" style="width:50%;" />{/if}

		{#if ready}<h1 in:fade={{ duration: 2000 }} style="margin-top:2.5%;">
				><b>Sponsors</b> and <b>Partners</b><span class="terminal">_</span>
			</h1>{/if}


			<div class="sponsors">
				{#if ready}<a in:fade={{ duration: 2000 }} href="http://www.ploiesti.ro/"
						><img
							src="primarie.png"
							alt="Primaria Municipiului Ploiesti"
							style="width:15% !important; margin-top:-5vh !important;"
						/></a
					>{/if}
				<br />
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://www.pfarma.ro/"
						><img src="farmaline.png" alt="Farmaline" style="width:40% !important;" /></a
					>{/if}
				{#if ready}<a
						in:fade={{ duration: 2000 }}
						href="https://www.intesrnational-alexander.ro/en/home/"
						><img
							src="alexander.png"
							alt="International Alexander"
							style="width:30% !important;"
						/></a
					>{/if}
				<br />
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://www.pufuletigusto.ro/en/"
						><img src="gusto.png" alt="Gusto Pufuleti" style="width:10% !important;" /></a
					>{/if}
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://www.audiolux.ro/"
						><img
							src="audiolux.png"
							alt="AudioLux"
							style="width:20% !important;"
						/></a
					>{/if}
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://superdentist.ro/"
						><img src="superdentist.png" alt="SuperDentist" style="width:25% !important;" /></a
					>{/if}
				<br />
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://ipad.ro/"
						><img src="ipad.png" alt="IPAD ROMANIA" style="width:10% !important;" /></a
					>{/if}
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://www.conpet.ro/"
						><img src="conpet.png" alt="Conpet" style="width:20% !important;" /></a
					>{/if}
				{#if ready}<a
						in:fade={{ duration: 2000 }}
						href="https://www.google.com/maps/place/Crisman+PiM/@44.9421177,25.9850561,15z/data=!4m2!3m1!1s0x0:0x7cd388e97b25c5dc?sa=X&ved=2ahUKEwjLusWtiIf3AhVNhP0HHeVWDuMQ_BJ6BAhJEAU"
						><img
							src="crisman.png"
							alt="criSman"
							style="width:20% !important;"
						/></a
					>{/if}
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://www.niko.com.ro/"
						><img
							src="niko.png"
							alt="Niko Romania"
							style="width:5% !important;"
						/></a
					>{/if}
				<br />
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://servtop.ro/"
						><img src="servtop.png" alt="Servtop Romania" style="width:20% !important;" /></a
					>{/if}
		
				{#if ready}<a
						in:fade={{ duration: 2000 }}
						href="https://www.google.com/maps/place/M%C4%83cel%C4%83rie+Tradi%C8%9Bionala+Pion/@44.9421402,25.9960646,15z/data=!4m5!3m4!1s0x0:0xe9d5e74823936fca!8m2!3d44.9421413!4d25.9960651"
						><img
							src="pion.png"
							alt="Pion Impex"
							style="width:10% !important;"
						/></a
					>{/if}
				<br />
				<br />
				<br />
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://natieprineducatie.ro/"
						><img src="brd.png" alt="Natie Prin Educatie" style="width:50% !important;margin-top:0 !important;" /></a
					>{/if}
				<br />
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://centrulexcelenta.com/"
						><img
							src="cex.png"
							alt="Centrul de Excelenta Prahova"
							style="width:10% !important;margin-top:0 !important;"
						/></a
					>{/if}
				{#if ready}<a in:fade={{ duration: 2000 }} href="http://www.cn-caragiale.ro/"
						><img src="cara.png" alt="CNILC" style="width:8% !important;" /></a
					>{/if}
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://www.facebook.com/info1robotics"
						><img
							src="educatie.png"
							alt="Performanta Prin Educatie"
							style="width:9% !important;margin-top:0 !important;"
						/></a
					>{/if}
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://sites.google.com/site/centrulinfo1/"
						><img
							src="info1project.png"
							alt="Proiectul infO1"
							style="width:25% !important;margin-top:0 !important;	"
						/></a
					>{/if}
			</div>

	
			<div class="linkssection">
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://www.instagram.com/info1robotics/"
						><img
							src="https://drive.google.com/uc?id=1cMI5UrBOrvltwZ090ys5m7wCe4c1u4fd"
							alt="INSTAGRAM"
						/></a
					>{/if}
				{#if ready}<a in:fade={{ duration: 2000 }} href="https://www.facebook.com/info1robotics/"
						><img
							src="https://drive.google.com/uc?id=1YDEBin_npoElopwus2CouhVJqNORE8aM"
							alt="FACEBOOK"
						/></a
					>{/if}
				{#if ready}<a
						in:fade={{ duration: 2000 }}
						href="https://www.youtube.com/channel/UC6PkNCRNEQOfKuciVltqzTQ"
						><img
							src="https://drive.google.com/uc?id=1HndKVFjySGNx1edEEH9OXP7zRnRA4qUG"
							alt="YOUTUBE"
						/></a
					>{/if}
				{#if ready}<a
						in:fade={{ duration: 2000 }}
						href="https://open.spotify.com/show/6glFbyo8OnIqih7RuPjB1e"
						><img
							src="https://drive.google.com/uc?id=1ki_ydOgY3Kz7qzI3m12DP1EgLvndMa6B"
							alt="SPOTIFY"
						/></a
					>{/if}
				{#if ready}<a in:fade={{ duration: 2000 }} href="mailto: info1robotics@gmail.com"
						><img
							src="https://drive.google.com/uc?id=17d8EWjB6gFm1NVgigRpdm1iHloEFQDIk"
							alt="EMAIL"
						/></a
					>{/if}
			</div>

	</div>

</html>

<style>
	/* Global CSS */

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

	/* Navigation */
	.spinning {

		position: fixed;
		bottom: 60vh;
		left: -40vw;
		margin: 20px;
		width: 100px;
		height: 100px;
z-index: 0;
		opacity: 30%;
		
	}

	.spinning img {
		width: 200vh;
		height: auto;
		position:relative;
		filter: invert(100%);

		transform-origin: 50% 50%;

		-webkit-animation-name: spin;
		-webkit-animation-duration: 2000ms;
		-webkit-animation-iteration-count: infinite;
		-webkit-animation-timing-function: linear;
		-moz-animation-name: spin;
		-moz-animation-duration: 10000ms;
		-moz-animation-iteration-count: infinite;
		-moz-animation-timing-function: linear;
		-ms-animation-name: spin;
		-ms-animation-duration: 10000ms;
		-ms-animation-iteration-count: infinite;
		-ms-animation-timing-function: linear;
		animation-name: spin;
		animation-duration: 10000ms;
		animation-iteration-count: infinite;
		animation-timing-function: linear;
	}

	@-ms-keyframes spin {
		from {
			-ms-transform: rotate(0deg);
		}
		to {
			-ms-transform: rotate(360deg);
		}
	}

	@-moz-keyframes spin {
		from {
			-moz-transform: rotate(0deg);
		}
		to {
			-moz-transform: rotate(360deg);
		}
	}

	@-webkit-keyframes spin {
		from {
			-webkit-transform: rotate(0deg);
		}
		to {
			-webkit-transform: rotate(360deg);
		}
	}

	@keyframes spin {
		from {
			transform: rotate(0deg);
		}
		to {
			transform: rotate(360deg);
		}
	}
	.nav {
		z-index: 1000;
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

	/* Mobile Navigation Menu */

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

	/* Splash Screen */

	.splashscreen {
		clip-path: polygon(0 0, 0 100%, 100% 100%, 100% 0);
		width: 100vw;
		height: 100vh;
		background-color: #39b44a;
		z-index: -2;
		overflow-x: hidden;
	}

	.splash-title {
		z-index: 2;
		box-sizing: border-box;
		padding-top: 10%;
		padding-left: 10%;
		position: absolute;
		top: 40%;
		-ms-transform: translateY(-50%);
		transform: translateY(-50%);
	}

	.splashscreen h1 {
		color: #15181e;
		text-align: unset;
		font-weight: 500;
		font-size: 8em;
		line-height: 0.4;
	}

	.splashscreen b {
		color: #d0d3e1;
	}

	.splash-title p {
		color: #15181e;
		margin-top: -10px;
		font-size: 2em;
		text-transform: uppercase;
	}

	.alignCAD {
		z-index: 2;
		width:20%;
		max-width: 100%;
    height: auto;
    width: auto\9;
		position: absolute;
		left: 50%;
		top: 50%;
		-ms-transform: translateY(-50%);
		transform: translateY(-50%);
	}
	@media only screen and (max-width: 1000px) {
		.alignCAD {
			left: 0%;
			width: 50%;
			top: 37.5%;
		}
		.splashscreen h1 {
			text-align: center;
		}
		.splash-title {
			text-align: center;
			top: 75%;
			margin-top: 3.5%;
			padding-top: 0;
			padding-left: 0;
			display: flex;
  			justify-content: center;
			font-size: 150%;
		}
		.splash-title h1 {
			font-size: 500%;
		}
		.aboutus h1 {
			font-size: 300%;
			margin-top: 10% !important;
		}
		.aboutus p {
			font-size: 200%;
		}
		.aboutus {
			height: 0;
		}
		.aboutus img {
			width: 75vw !important;
		}
		.splashscreen img {
			margin-bottom: 5vh;
		}
		.linkssection {
			height: 4vh !important;
		}
		.aboutus {
			height: 490vh !important;
		}
	}

	.alignCAD img {
		width: 200%;
	}

	/* About Us Section */

	.aboutus {
		width: 100vw;
		background-color: #15181e;
		z-index: 9999;
		color: #d0d3e1;
		height: 650vh;
	}
	.aboutus h1 {
		text-align: center;
		text-decoration: underline;
		text-underline-offset: 5px;
	}
	.aboutus b {
		color: #0b6623;
	}
	.aboutus p {
		text-align: center;
		margin-top: 5vh;
		margin-bottom: 5vh;
		margin-left: 15vw;
		margin-right: 15vw;
	}
	.aboutus img {
		display: block;
		margin-left: auto;
		margin-right: auto;
		width: 30vw;
		border: 3px solid #d0d3e1;
		border-radius: 16px;
	}
	.sponsors img{
		display:unset !important;
		border: 0px !important;
		border-radius: 0 !important;
		margin-top: 2.5vh !important;
		margin-left: 2.5vh !important;
		margin-right: 2.5vh !important;
		margin-bottom: 2.5vh !important;
	}
	.linkssection img{
		display:unset !important;
		border: 0px !important;
		border-radius: 0 !important;
	}
	.sponsors {
		position: relative !important;
		text-align: center !important;
		margin-top: 10vh !important;
		width: 100vw !important;
	}
	.linkssection {
		position: relative !important;
		margin-top: 5vh !important;
	}
	.linkssection img {
		width: 19.5vw !important;
		height: auto !important;
	}
</style>
