<template>
	<div class="skill">
		<h5 class="language">{{ language }}</h5>
		<div class="d-flex align-items-center">
			<div class="percent">
				<div :style="{ '--percent': `${percent.toString()}%` }"></div>
			</div>
			<span class="ml-3">{{ `${percent.toString()}%` }}</span>
		</div>
	</div>
</template>

<script>
export default {

	name: 'SkillPercent',

	props: {
		language: {
			type: String,
			required: true
		},
		percent: {
			type: Number,
			default: 0
		}
	},

	data () {
		return {

		}
	}
}
</script>

<style lang="css" scoped>
.skill {
	margin-bottom: 20px;
}

.language {
	font-size: 20px;
}

.percent {
	width: 100%;
	padding: 3px;
	border-radius: 50px;
	background-color: #fff;
}

.percent div {
	border-radius: 50px;
	width: var(--percent);
	height: 10px;
	background-color: var(--color1); 
}

.percent + span {
	font-size: 18px;
	color: var(--color2);
}
</style>