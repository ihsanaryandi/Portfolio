<template>
	<div id="about">
		<div class="container">
			<div class="row">
				<div class="col-lg-6 p-4">
					<div class="my-photo">
						<img :src="myPhoto">
					</div>
				</div>
				<div class="col-lg-6 p-4">
					<div class="about-me">
						<h1>About me</h1>
						<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
						tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
						quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
						consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
						cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
						proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
					</div>		
				</div>
			</div>
		</div>
	</div>
</template>

<script>

import myPhoto from '../../assets/my-photo.jpg'

export default {

	name: 'About',

	data () {
		return {
			myPhoto
		}
	}
}
</script>

<style lang="css" scoped>

#about {
	margin-bottom: 150px;
	padding: 20px 0;
	background-color: var(--color1);
}

.my-photo {
	position: relative;
	width: 100%;
	height: 500px;
	display: flex;
	justify-content: center;
	align-items: center;
	background-color: var(--bg-color);
	z-index: 1;
}

.my-photo img {
	width: 300px;
	height: 350px;
	object-fit: cover;
	box-shadow: 15px 15px 0px yellow,
				-15px -15px 0px salmon;
}

.about-me {
	width: 100%;
	height: 100%;
	color: #fff;
	padding: 30px 0;
}

.about-me h1 {
	font-size: 3em;
}

</style>

