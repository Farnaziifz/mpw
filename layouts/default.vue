<template>
	<div class="fz__parent">
		<div class="container">
			<div class="fz_sub_container">
				<div class="fz__box">
					<div class="fz__info-box">
						<div class="fz__container">
							<div class="fz__image"></div>
							<div class="fz__name">
								<h2>Farnaz Farzipour</h2>
							</div>
							<div class="fz__title">
								<h6>Front-End Developer</h6>
							</div>
							<div class="fz__social">
								<img src="~/assets/icons/instagram.svg" alt="" />
								<img src="~/assets/icons/telegram.png" alt="" />
								<img src="~/assets/icons/telegram.png" alt="" />
								<img src="~/assets/icons/telegram.png" alt="" />
							</div>
							<div class="fz__button">
								<button class="fz__cv_button">
									<a href="">Download CV</a>
								</button>
							</div>
						</div>
						<div class="fz__copyright">© 2020 All rights reserved.</div>
					</div>
					<div class="fz__contect-box_container">
						<Nuxt class="fz__contect-box" />
					</div>
				</div>
				<div class="fz__navigator"></div>
			</div>
		</div>
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

	.container {
		height: 100%;
	}
	.fz_sub_container {
		display: flex;
		height: 100%;
	}

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
			justify-content: space-between;
			padding: 20px 10px;

			.fz__container {
				display: flex;
				flex-direction: column;
				align-items: center;
				justify-content: center;
				.fz__image {
					position: relative;
					width: 200px;
					height: 200px;
					background-color: #fff;
					border-radius: 50%;
					border: 3px solid #fff;
					margin-top: 50px;
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
					margin-top: 30px;
					width: 100%;
					display: flex;
					justify-content: center;

					img {
						width: 20px;
						height: 20px;
						object-fit: contain;
						margin-right: 10px;
					}
				}
				.fz__cv_button {
					width: 200px;
					height: 50px;
					border-radius: 30px;
					border: 2px solid #fff;
					background-color: transparent;
					margin-top: 50px;
					box-shadow: 0 0 30px -5px rgb(0 0 0 / 15%);
					a {
						width: 100%;
						height: 100%;
						text-decoration: none;
						color: #fff !important;
						&:hover {
							text-decoration: none;
							color: #fff;
						}
					}
				}
			}

			.fz__copyright {
				color: #fff;
				width: 100%;
				font-size: 14px;
				text-align: center;
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
