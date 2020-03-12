<template>
	<header id="header">
		<div class="container">
			<div class="my-name">
				<a href="#">Ihsan Aryandi</a>
			</div>
			<div class="row align-items-center">
				<div class="col-lg-6 col-md-6 mb-4">
					<h1 class="title">Web Developer</h1>
					<p class="text">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
					tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
					quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
					consequat.</p>
				</div>
				<div class="col-lg-6 col-md-6 text-center">
					<div class="illustration">
						<img :src="illustration2" alt="illustration">
					</div>
				</div>
			</div>
		</div>
	</header>
</template>

<script>

import illustration2 from '../../assets/illustration2.svg'

export default {

	name: 'Header',

	data () {
		return {
			illustration2
		}
	}
}
</script>

<style lang="css" scoped>

#header {
	height: 100vh;
	margin-bottom: 50px;
}

.my-name {
	padding: 15px 0;
	margin-bottom: 40px;
}

.my-name a {
	font-size: 28px;
	color: #eee;
	letter-spacing: 1.5px;
	/*font-weight: ;*/
	text-decoration: none;
}

.title {
	font-weight: 200;
	font-size: 50px;
	margin-bottom: 10px;
}

.text {
	color: var(--color2);
}

.illustration {
	max-width: 500px;
}

.illustration img {
	width: 100%;
}

</style>












