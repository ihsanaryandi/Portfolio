<template>
	<div id="header">
		<Navbar />
		<div class="container">
			<div class="row">
				<div class="col-lg-6">
					<div class="opening">
						<h1>Web Developer</h1>
						<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
						tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
						quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
						consequat.</p>
						<div class="cta">
							<a href="#">Hire Me</a>
							<a class="outline" href="#">See My Works</a>
						</div> 
					</div>
				</div>
				<div class="col-lg-6">
					<div class="illustration">
						<img :src="illustration">
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>

// Components
import Navbar from './Navbar'

// Assets
import illustration from '../../assets/illustration1.svg'

export default {

	name: 'Header',

	components: {
		Navbar
	},

	data () {
		return {
			illustration
		}
	}
}
</script>

<style lang="css" scoped>

#header {
	margin-bottom: 150px;
}

.opening {
	padding: 10px 0;
}

.opening h1 {
	font-size: 3em;
	font-weight: 200;
}

.opening p {
	color: #888;
}

.cta {
	margin-top: 40px;
}

.cta a {
	display: inline-block;
	background-color: var(--color1);
	color: #fff;
	font-size: 20px;
	padding: 8px 30px;
	margin-right: 15px;
	border-radius: 5px;
	text-decoration: none;
	border: 2px solid var(--color1);
	margin-bottom: 10px;
	transition: .2s;
}

.cta a:active {
	opacity: .8;
}

.cta a:last-child {
	margin: 0;
}

.cta a.outline {
	background-color: #fff;
	color: var(--color1);
}

.cta a:hover {
	background-color: #fff;
	color: var(--color1);	
}

.cta a.outline:hover {
	background-color: var(--color1);
	color: #fff;
}

.illustration {
	width: 90%;
	margin: auto;
}

.illustration img {
	width: 100%;
}

@media only screen and (max-width: 990px) {
	.opening {
		margin-bottom: 50px;
	}
}

</style>














