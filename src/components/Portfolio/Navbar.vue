<template>
	<nav id="navbar">
		<div class="container">
			<div class="my-name">
				<a href="#">{Ihsan Aryandi}</a>			
			</div>
			<div class="items" v-bind:class="{ open }">
				<div class="close" @click="closeMenu">&times;</div>
				<ul>
					<li>
						<a class="item-link" href="#">Home</a>
					</li>
					<li>
						<a class="item-link" href="#">About</a>
					</li>
					<li>
						<a class="item-link" href="#">Skills</a>
					</li>
					<li>
						<a class="item-link" href="#">Contact</a>
					</li>
				</ul>
			</div>
			<div class="burger-menu">
				<button type="button" @click="openMenu">
					<span></span>
				</button>
			</div>
		</div>
	</nav>
</template>

<script>
export default {

	name: 'Navbar',

	data () {
		return {
			open: false
		}
	},

	methods: {
		openMenu() {
			this.open = true
		},

		closeMenu() {
			this.open = false
		}
	},

	created() {

	}
}
</script>

<style lang="css" scoped>

nav {
	min-height: 15vh;
	margin-bottom: 50px;
	background-color: #fff;
}

.container {
	display: flex;
	justify-content: space-between;
	align-items: center;
	height: 15vh;
}

.my-name {
	font-size: 24px;
}

.my-name a {
	text-decoration: none;
	color: var(--color1);
}

.items .close {
	display: none;
}

.items ul {
	display: flex;
	margin: 0;
	list-style: none;
}

.items ul li {
	padding: 5px 10px;
	margin-left: 10px;
}

.item-link {
	color: var(--color3);
	text-transform: uppercase;
	font-weight: 200;
}

.burger-menu {
	display: none;
}

.burger-menu button {
	position: relative;
	width: 30px;
	height: 25px;
	border: none;
	outline: none;
	background-color: transparent;
}

.burger-menu button:hover span {
	--line-color: #555;
}

.burger-menu button:hover span:before {
	right: 50%;
}

.burger-menu button:hover span:after {
	left: 50%;
}

.burger-menu span {
	--line-color: #ccc;
}

.burger-menu span,
.burger-menu span::before,
.burger-menu span::after {
	display: block;
	width: 100%;
	height: 4px;
	border-radius: 10px;
	background-color: var(--line-color);
	transition: .3s;
}

.burger-menu span::before {
	content: '';
	position: absolute;
	top: 0;
	right: 0;
	width: 50%;
}

.burger-menu span::after {
	content: '';
	position: absolute;
	bottom: 0;
	left: 0;
	width: 50%;
}

@media only screen and (max-width: 770px) {
	.items {
		position: fixed;
		top: 0;
		left: 0;
		z-index: 1000;
		width: 100%;
		height: 100%;
		background-color: var(--color3);
		transform: translateY(100%);
		transition: .3s ease-out;
	}

	.items.open {
		transform: translateY(0);
	}

	.items .close {
		display: inline-block;
		position: absolute;
		top: 25px;
		right: 25px;
		font-size: 30px;
		color: #fff;
		cursor: pointer;
		user-select: none;
	}

	.items ul {
		min-height: 100vh;
		justify-content: center;
		align-items: center;
		flex-direction: column;
	}

	.items ul li {
		margin-left: 0;
		margin: 10px 0;
	}

	.item-link {
		font-size: 24px;
		color: #fff;
	}

	.burger-menu {
		display: block;
	}
}

</style>




















