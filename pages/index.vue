<template>
	<div class="fz__main_about">
		<h1>Farnaz Farzipour</h1>
		<h2>Front End Developer</h2>
	</div>
</template>

<script>
export default {
	transition: 'page',
};
</script>

<style lang="scss" scoped>
.fz__main_about {
	width: 100%;
	height: 100%;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	h1 {
		font-weight: bold;
	}
	h2 {
		color: rgb(145, 145, 145);
	}
}
</style>
