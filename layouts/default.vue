<template>
	<div class="fz__parent">
		<div class="fz__box">
			<div class="fz__info-box">
				<div class="fz__image"></div>
				<div class="fz__name">
					<h2>Farnaz Farzipour</h2>
				</div>
				<div class="fz__title">
					<h6>Front-End Developer</h6>
				</div>
				<div class="fz__social">
					<img src="~/assets/icons/instagram.svg" alt="" />
				</div>
				<div class="fz__button"></div>
			</div>
			<div class="fz__contect-box_container">
				<Nuxt class="fz__contect-box" />
			</div>
		</div>
		<div class="fz__navigator"></div>
	</div>
</template>
<script>
export default {
	transition: 'page',
};
</script>

<style lang="scss" scoped>
.fz__parent {
	width: 100%;
	height: 100vh;
	background-color: #f7e9ff;
	padding: 10vh 120px;
	display: flex;

	.fz__navigator {
		height: 300px;
		width: 70px;
		background-color: #fff;
		border-radius: 35px;
		margin-left: 20px;
		box-shadow: 0 0 30px -5px rgb(0 0 0 / 15%);
	}

	.fz__box {
		width: 100%;
		height: 100%;
		background-color: #751af6;
		border-radius: 20px;
		display: flex;
		box-shadow: 0 0 30px -5px rgb(0 0 0 / 15%);
		.fz__contect-box_container {
			width: 100%;
		}
		.fz__info-box {
			width: 500px;
			height: 100%;
			display: flex;
			flex-direction: column;
			align-items: center;
			justify-content: center;
			padding: 10px;
			.fz__image {
				position: relative;
				width: 250px;
				height: 250px;
				background-color: #fff;
				border-radius: 50%;
				border: 3px solid #fff;
			}
			.fz__name {
				margin-top: 20px;
				h2 {
					color: #fff;
					font-weight: bold;
				}
			}
			.fz__title {
				h6 {
					color: #fff;
					margin-top: 10px;
				}
			}
			.fz__social {
				img {
					width: 30px;
					height: 30px;
					object-fit: contain;
				}
			}
		}

		.fz__contect-box {
			width: 100%;
			height: 100%;
			background-color: #fff;
			border-radius: 20px;
		}
	}
}
</style>
