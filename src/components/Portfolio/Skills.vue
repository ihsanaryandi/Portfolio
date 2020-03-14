<template>
	<div id="skills">
		<h1 class="skills-display">Programming Skills</h1>
		<div class="container">
			<div class="card">
				<h1>Languages</h1>
				<SkillPercent language="HTML" :percent="90" />
				<SkillPercent language="CSS" :percent="95" />
				<SkillPercent language="Javasript" :percent="92" />
				<SkillPercent language="PHP" :percent="80" />
			</div>	
		</div>
	</div>
</template>

<script>

import SkillPercent from './SkillPercent'

export default {

	name: 'Skills',

	components: {
		SkillPercent
	},

	data () {
		return {

		}
	}
}
</script>

<style lang="css" scoped>

#skills {
	position: relative;
	overflow: hidden;
	min-height: 80vh;
	padding: 80px 0;
	background-color: #fff;
}

.skills-display {
	font-size: 8em;
	display: inline-block;
	text-transform: uppercase;
	position: absolute;
	top: 0;
	left: 0;
	font-weight: bold;
	color: #aaa;
	font-style: italic;
	max-width: 1000px;
}

.card {
	max-width: 550px;
	width: 95%;
	background-color: rgba(240, 240, 255, .8);
	margin-left: auto;
	border: none;
	padding: 50px;
	box-shadow: 25px 25px 16px rgba(0, 0, 0, 0.15);
}

.card h1 {
	text-align: center;
	margin-bottom: 30px;
}

</style>

