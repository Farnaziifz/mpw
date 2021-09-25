<template>
	<div class="fz__main_about">
		<h1><span>About </span><span class="color">Me</span></h1>
		<div class="fx__about_content mb-3">
			<div class="row">
				<div class="col-lg-12">
					<p class="fz__about_text">
						Another Front-End developer with 4 years experience in various projects, I have a lot of
						intrests in technology and developing, and the code becomes an important part of my
						life. addicted to solving challenges and always worrying about deadline. I'm creative
						and Self-development. One of the my positive point is that I never give up and have
						desire to Win.
					</p>
				</div>
			</div>
		</div>

		<!-- section 2 -->

		<div class="fz__ido mt-4">
			<h1><span>What's My</span> <span class="color">Skills</span></h1>
			<div class="fz__skill_container">
				<div class="item" v-for="item in skils" :key="item.id">
					<span>{{ item.name }}</span>
				</div>
			</div>
		</div>
		<div class="fz__ido mt-4">
			<h1><span>What's My</span> <span class="color">Skills</span></h1>
			<div class="row">
				<div class="col-gl-6"></div>
				<div class="col-lg-6"></div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	transition: 'page',
	data() {
		return {
			skils: [
				{
					id: 1,
					name: 'HTML & HTML5',
				},
				{
					id: 2,
					name: 'CSS & CSS3',
				},
				{
					id: 3,
					name: 'Pug',
				},
				{
					id: 4,
					name: 'Bootstrap',
				},
				{
					id: 5,
					name: 'SASS',
				},
				{
					id: 6,
					name: 'JavaScript',
				},
				{
					id: 7,
					name: 'ECMA Script',
				},
				{
					id: 8,
					name: 'VueJS',
				},
				{
					id: 9,
					name: 'PWA',
				},
				{
					id: 10,
					name: 'Gulp',
				},
				{
					id: 11,
					name: 'Linux',
				},
				{
					id: 12,
					name: 'Scrum',
				},
				{
					id: 12,
					name: 'NuxtJS',
				},
			],
		};
	},
};
</script>

<style lang="scss" scoped>
.fz__main_about {
	padding: 40px 20px;
	h1 {
		font-size: 30px;
		font-weight: bold;
		position: relative;
		display: inline-block;
		&:after {
			position: absolute;
			opacity: 0.45;
			top: 10px;
			left: 90%;
			content: '';
			height: 30px;
			width: 50px;
			background-image: -webkit-repeating-radial-gradient(
				center center,
				#751af6,
				#751af6 1px,
				transparent 0px,
				transparent 100%
			);
			background-image: -moz-repeating-radial-gradient(
				center center,
				#751af6,
				#751af6 1px,
				transparent 0px,
				transparent 100%
			);
			background-image: -ms-repeating-radial-gradient(
				center center,
				#751af6,
				#751af6 1px,
				transparent 0px,
				transparent 100%
			);
			-webkit-background-size: 6px 6px;
			-moz-background-size: 6px 6px;
			background-size: 6px 6px;
			z-index: 0;
		}

		.color {
			color: #751af6;
		}
	}

	.fx__about_content {
		width: 100%;
		margin-top: 40px;
		.fz__about_text {
			text-align: justify;
			font-size: 16px;
			padding: 0 20px;
		}
		.item {
			margin-bottom: 10px;
			.title {
				font-weight: bold;
				color: #751af6;
				margin-right: 10px;
			}
		}
	}

	.fz__skill_container {
		width: 100%;
		display: flex;
		justify-content: center;
		margin-top: 40px;
		margin-bottom: 100px;
		flex-wrap: wrap;
		.item {
			width: 80px;
			height: 80px;
			border: 2px solid #751af6;
			border-radius: 50%;
			display: flex;
			justify-content: center;
			align-items: center;
			text-align: center;
			margin: 5px;
			background-color: #f7e9ff;

			span {
				font-weight: bold;
				font-size: 14px;
				color: #8349d4;
			}
		}
	}
}
</style>
