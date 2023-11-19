<script>

</script>

<nav>
    <div class="nav-logo">
        <a href="#">
            <img src="" alt="" />
        </a>
    </div>

    <ul class="nav-links">
        <li class="link"><a href="#">Home</a></li>
        <li class="link"><a href="#">Features</a></li>
        <li class="link"><a href="#">About</a></li>
    </ul>
</nav>

<style>
nav {
	max-width: 129px;
	margin: auto;
	padding: 2rem 1rem;
	display: flex;
	align-items: center;
	justify-content: space-between;
	gap: 2rem;
}

.nav-logo {
	max-width: 100px;
}

.nav-links {
	list-style: none;
	display: flex;
	align-items: center;
	gap: 3rem;
}

.link a {
    text-decoration: none;
	position: relative;
	padding-bottom: 0.75rem;
	color: #fff;
}

.link a::after {
	content: '';
	position: absolute;
	height: 2px;
	width: 0;
	bottom: 0;
	left: 0;
	background-color: #1d4ed8;
	transition: all 0.3s ease;
}

.link a:hover::after {
	width: 70%;
}
</style>