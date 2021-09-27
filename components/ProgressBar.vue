<template>
	<div class="fz__progress">
		<div class="fz__label">{{ name }}:</div>
		<div class="fz__progress-container">
			<div class="fz__count" :style="{ width: count + '%', background: color }"></div>
		</div>
	</div>
</template>

<script>
export default {
	data() {
		return {
			count: 0,
		};
	},
	props: {
		percent: {
			default: 0,
			type: Number,
		},
		color: {
			default: '#751af6',
			type: String,
		},
		name: String,
	},
	mounted() {
		this.count = this.percent;
	},
};
</script>

<style lang="scss" scoped>
.fz__progress {
	width: 100%;
	// display: flex;
	// align-items: center;
    margin-bottom: 10px;
	.fz__label {
		margin-right: 10px;
		font-weight: bold;
        font-size: 14px;
        width: 25%;
	}
	.fz__progress-container {
		width: 100%;
		height: 15px;
		border: 1px solid #751af6;
		border-radius: 20px;
		padding: 3px;
		.fz__count {
			height: 100%;
			border-radius: 20px;
			transition: all 1s;
		}
	}
}
</style>
