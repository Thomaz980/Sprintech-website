<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
	import Nav from '../components/Nav.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<div class="body">
	<Nav />

	<header class="conteiner">
		<div class="content">
			<span class="blur"></span>
			<span class="blur"></span>
			<h4>CREATE YOUR SITE A PRO</h4>
			<h1><span>Sprintech</span>, Desenvolvimento de Software</h1>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
				quibusdam, voluptatum, quos, voluptate quia quae dolorum
				accusantium.
			</p>
			<button class="btn">Get Started</button>
		</div>
		<div class="image">
			<img src="#">
		</div>
	</header>

	<section class="conteiner">
		<h2 class="header">OUR FEATURES</h2>
		<div class="features">
			<div class="card">
				<span><i class="icon"></i></span>
				<h4>Free Tutorials</h4>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
					quibusdam, voluptatum, quos, voluptate quia quae dolorum
					accusantium, voluptat.
				</p>
				<a href="#">Join Now <i class="#"></i></a>
			</div>
			<div class="card">
				<span><i class="icon"></i></span>
				<h4>Free Tutorials</h4>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
					quibusdam, voluptatum, quos, voluptate quia quae dolorum
					accusantium, voluptat.
				</p>
				<a href="#">Join Now <i class="#"></i></a>
			</div>
			<div class="card">
				<span><i class="icon"></i></span>
				<h4>Free Tutorials</h4>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
					quibusdam, voluptatum, quos, voluptate quia quae dolorum
					accusantium, voluptat.
				</p>
				<a href="#">Join Now <i class="#"></i></a>
			</div>
		</div>
	</section>

	<!-- Contato -->

	<footer>
		<span class="blur"></span>
		<span class="blur"></span>
		<div class="column">
			<div class="logo">
				<img src="#" alt="">
			</div>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
				quibusdam, voluptatum.
			</p>
			<div class="socials">
				<a href="#"><i class="ri-instagram-line"></i></a>
				<a href="#"><i class=""></i></a>
				<a href="#"><i class=""></i></a>
			</div>
		</div>
		<div class="column">
			<h4>Company</h4>
			<a href="">Business</a>
			<a href="">Partnership</a>
			<a href="">Networking</a>
		</div>
		<div class="column">
			<h4>About Us</h4>
			<a href="">Business</a>
			<a href="">Partnership</a>
			<a href="">Networking</a>
		</div>
		<div class="column">
			<h4>Contect</h4>
			<a href="">Business</a>
			<a href="">Partnership</a>
			<a href="">Networking</a>
		</div>
	</footer>

	<div class="copyright">
		<p>&copy; 2021 Sprintech. All Rights Reserved.</p>
	</div>
</div>

<style>

img {
	width: 100%;
	display: flex;
}

a {
	text-decoration: none;
}

.body {
	font-family: 'Popins', sans-serif;
	background-color: #181818;
}


.btn {
	padding: 1rem 2rem;
	font-size: 1rem;
	color: #fff;
	background-color: #1d4ed8;
	border-radius: 5px;
	cursor: pointer;
	transition: all 0.3s ease;
}

.btn:hover {
	background-color: #1e40af;
}

.container {
	max-width: 120px;
	margin: auto;
	padding: 5rem 2rem;
}

.blur{
	position: absolute;
	box-shadow: 0 0 1000px 50px #1d4ed8;
	z-index: -100;
}

header {
	position: relative;
	padding-top: 2rem;
	display: grid;
	grid-template-columns: repeat(2, 1fr);
	gap: 2rem;
}

header .content h4 {
	margin-bottom: 1rem;
	color: #ccc;
	font-size: 1rem;
	font-weight: 600;
}

header .content h1 {
	color: #fff;
	margin-bottom: 1 rem;
	font-size: 3rem;
	font-weight: 700;
	line-height: 4rem;
}

header .content h1 span {
	-webkit-text-fill-color: transparent;
	-webkit-text-stroke: 1px #fff;
}

header .content p {
	color: #ccc;
	margin-bottom: 2rem;
}

header .image {
	position: relative;
}

header .image::before {
	content: "o";
	position: absolute;
	top: 0;
	left: 0;
	transition: translateX(-50%);
	font-size: 38rem;
	line-height: 20rem;
	color: #1d4ed8;
	opacity: 0.2;
	z-index: -100;;
}

header .image img {
	max-width: 600px;
	margin: auto;
}

section .header {
	color: #fff;
	text-align: center;
	font-weight: 600;
}

.features {
	margin-top: 4rem;
	display: grid;
	grid-template-columns: repeat(4, 1fr);
	grid: 2rem;
}

.features .card {
	background-color: #27272a;
	padding: 1rem;
	border: 2px solid transparent;
	border-radius: 15px;
	transition: all 0.3s ease;
}

.features .card:hover {
	background-color: #323232;
	border-color: #fff;
}

.features .card span {
	display: inline-block;
	background-color: #1d40af;
	padding: 2px 9px;
	margin-bottom: 1rem;
	font-size: 1.75rem;
	color: #fff;
	border-radius: 5px;
}

.features .card h4 {
	margin-bottom: 0.5rem;
	color: #fff;
	font-size: 1.2rem;
	font-weight: 600;
}

.features .card p {
	color: #ccc;
	margin-bottom: 1rem;
}

.features .card a {
	color: #fff;
	transition: all 0.3s ease;
}

.features .card a:hover {
	color: #1e40af;
}

.sub-header {
	max-width: 600px;
	margin: auto;
	text-align: center;
	color: #ccc;
}

footer {
	position: relative;
	display: grid;
	padding: 5rem 2rem;
	grid-template-columns: repeat(3, 1fr);
	gap: 2rem;
}

footer .column .logo {
	max-width: 100px;
	margin-bottom: 2rem;
}

footer .column p {
	color: #ccc;
	margin-bottom: 2rem;
}

footer .column .socials {
	display: flex;
	align-items: center;
	gap: 1rem;
}

footer .column .socials a {
	color: #fff;
	font-size: 1.5rem;border: 1px solid #ccc;
	padding: 5px 10px;
	font-size: 1.25rem;
	border-radius: 100%;
	transition: all 0.3s ease;
}

footer .column .socials a:hover {
	color: #fff;
	background-color: #1d4ed8;
	border-color: #1d4ed8;
}

footer .column h4 {
	color: #fff;
	margin-bottom: 2rem;
	font-size: 1.2rem;
	font-weight: 500;
}

footer .column > a {
	color: #ccc;
	margin-bottom: 1rem;
	display: block;
	transition: all 0.3s ease;
}

footer .column > a:hover {
	color: #1d4ed8;
}

.copyright {
	max-width: 1200px;
	margin: auto;
	padding: 1rem;
	text-align: center;
	color: #fff;
}

@media (width < 900px){
	.nav-links {
		display: none;
	}
	header{
		grid-template-columns: repeat(1, 1fr);
	}
	header .image {
		grid-area: 1/1/2/2;
	}
	.features {
		grid-template-columns: repeat(2, 1fr);
	}
	.pricing {
		grid-template-columns: repeat(2, 1fr);
	}
	footer {
		grid-template-columns:  1fr 200px;
	}
}

@media (width < 600px){
	header .image::before {
		display: none;
	}
	.features {
		grid-template-columns: repeat(1, 1fr);
	}
	.pricing {
		grid-template-columns: repeat(1, 1fr);
	}
	footer {
		grid-template-columns: 1fr 150px;
	}
}
</style>
