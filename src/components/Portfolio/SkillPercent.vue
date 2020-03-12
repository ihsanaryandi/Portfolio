<template>
	<div class="skill-percent">
		<h5>{{ skillName }}</h5>
		<div class="d-flex align-items-center mb-2">
			<div class="percent-bar">
				<div :style="{ '--percent': `${percent}%`, '--colorBar': colorBar }"></div>
			</div>
			<span>{{ `${percent}%` }}</span>
		</div>	
	</div>
</template>

<script>
export default {

	name: 'SkillPercent',

	data () {
		return {

		}
	},

	props: {
		skillName: {
			type: String,
			required: true
		},
		percent: {
			type: Number,
			default: 0
		},
		colorBar: {
			type: String,
			default: 'lightgreen'
		}
	}
}
</script>

<style lang="css" scoped>

h5 {
	color: var(--color2);
}

.percent-bar {
	width: 100%;
	height: 5px;
	background-color: var(--color2);
	border-radius: 20px;
}

.percent-bar div {
	width: var(--percent);
	height: 100%;
	border-radius: 20px;
	background-color: var(--colorBar);
	box-shadow: 0 0 20px var(--colorBar);
}

.percent-bar + span {
	padding: 0 20px;
	font-size: 18px;
}

</style>