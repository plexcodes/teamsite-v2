<script>
	import { fade, fly, slide } from 'svelte/transition'; // Svelte - Transitions
	import { onMount } from 'svelte'; // Svelte - JS Load
	// import Particles from 'svelte-particles'; // Background Typescript-Based tsParticles Library
	// import { inview } from 'svelte-inview/src';
	// let isInView;
	let ready = false;
	onMount(() => (ready = true));
</script>

<html lang="en">
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
			<a href="/3d" class="nav-active">>3D View<span class="terminal">_</span></a>
			<a href="/members">>Members<span class="terminal">_</span></a>
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
			<li><a href="/3d">>3D View<span class="terminal">_</span></a></li>
		</ul>
	</div>

	<div class="background">
		<div class="mobiletitle">
			{#if ready}<a
					href="https://gmail759693.autodesk360.com/shares/public/SH35dfcQT936092f0e43fd8b5363d7a3dc57"
					><h1 in:fly={{ y: -2000, duration: 2000 }}>
						Click here to see the <b>3D CAD</b> of our
						<b>2022 FTC Freight Frenzy World Championship Robot!</b>
					</h1></a
				>{/if}
		</div>
		<div class="title">
			{#if ready}<h1 in:fly={{ y: -2000, duration: 2000 }}>
					Check out the <b>3D CAD</b> of our
					<b>2022 FTC Freight Frenzy <br /> World Championship Robot!</b>
				</h1>{/if}
		</div>
		{#if ready}<div in:fly={{ y: 2000, duration: 2000 }} class="spinning">
				<img src="vortex.svg" alt="vortex" />
			</div>{/if}

		<div class="cadframe">
			<!-- svelte-ignore a11y-missing-attribute -->
			{#if ready}<iframe
					in:fade={{ duration: 5000 }}
					src="https://gmail759693.autodesk360.com/shares/public/SH35dfcQT936092f0e43ebe71ccd56b6222f?mode=embed"
					allowfullscreen="true"
					webkitallowfullscreen="true"
					mozallowfullscreen="true"
					frameborder="0"
				/>{/if}
		</div>
	</div>
</html>

<style>
	:global(body) {
		scroll-behavior: smooth;
		font-family: 'orbitron';
		overflow-x: hidden;
		margin: 0;
		padding: 0;
		background-repeat: no-repeat;
		background-size: cover;
		background-position: center;
	}

	.cadframe {
		width: 75vw;
		height: 60vh;
		position: absolute;
		left: 50%;
		top: 60%;
		-webkit-transform: translate(-50%, -50%);
		transform: translate(-50%, -50%);
	}

	@media only screen and (max-width: 1000px) {
		.cadframe {
			height: 75vh;
		}
		.title {
			top: 12% !important;
			font-size: 120% !important;
		}
	}
	.cadframe iframe {
		position: absolute;
		top: 0;
		bottom: 0;
		left: 0;
		right: 0;
		width: 100%;
		height: 100%;
	}
	a {
		color: #15181e;
	}
	.title {
		text-align: center;
		z-index: 1;
		position: absolute;
		font-size: 0.8em;
		left: 50%;
		top: 19%;
		-webkit-transform: translate(-50%, -50%);
		transform: translate(-50%, -50%);
	}

	.mobiletitle {
		visibility: hidden;
		text-align: center;
		padding-left: 0 !important;
		z-index: 1;
		position: absolute;
		font-size: 1.5em;
		left: 50%;
		top: 50%;
		-webkit-transform: translate(-50%, -50%);
		transform: translate(-50%, -50%);
	}

	b {
		color: #d0d3e1;
	}

	.background {
		background-color: #39b44a;
		width: 100vw;
		height: 100vh;
	}

	.spinning {
		position: fixed;
		bottom: 80vh;
		left: 0vw;
		margin: 20px;
		width: 100px;
		height: 100px;
		z-index: 0;
		opacity: 30%;
	}

	.spinning img {
		width: 200vh;
		height: auto;
		position: relative;
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

	@import url('https://fonts.googleapis.com/css?family=Poppins:400,500,600,700&display=swap');

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
</style>
