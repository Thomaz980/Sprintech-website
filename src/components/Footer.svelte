<script>
	import Git from '../lib/images/icons8-github.svg';
	import Insta from '../lib/images/icons8-insta.svg';
	import Linkedin from '../lib/images/icons8-linkedin.svg';
    
</script>

<footer>
    <span class="blur"></span>
    <span class="blur"></span>
    <div class="column">
        <div class="logo">
            <img src="#" alt="">
        </div>
        <p>
            Desenvolvimento e aplicações web.
        </p>
        <div class="socials">
            <a href="#"><img src={Git}></a>
            <a href="#"><img src={Insta}></a>
            <a href="#"><img src={Linkedin}></a>
        </div>
    </div>
    <div class="column">
        <h4>Company</h4>
        <a href="#">Business</a>
        <a href="#">Partnership</a>
        <a href="#">Networking</a>
    </div>
    <div class="column">
        <h4>About Us</h4>
        <a href="#">Business</a>
        <a href="#">Partnership</a>
        <a href="#">Networking</a>
    </div>
    <div class="column">
        <h4>Contect</h4>
        <a href="#">Business</a>
        <a href="#">Partnership</a>
        <a href="#">Networking</a>
    </div>
</footer>

<style>

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

img {
    width: 30px;
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
</style>