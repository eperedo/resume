<template>
	<section class="skill-item">
		<p class="skill-title">
			{{skill.title}}
		</p>
		<p class="skill-description">
			{{skill.description}}
		</p>
		<div class="skill-percent">
			<div class="skill-percent-circle">
				<div class="skill-percent-circle-opacity"></div>
			</div>
		</div>
	</section>
</template>

<script>
export default {
	name: 'profile-skill',
	props: {
		skill: {
			type: Object,
			required: true,
		},
	},
};
</script>

<style lang="scss" scoped>
.skill-item {
	display: flex;
	flex-direction: column;
	margin-top: 8%;

	.skill-description {
		color: map-get($colors, black);
		font-size: map-get($sizes, medium);
		line-height: 25px;
		margin-bottom: 7%;
		width: 319px;
	}

	.skill-title {
		font-family: map-get($fonts, black);
		font-size: map-get($sizes, large);
		margin: 0;
	}

	.skill-percent {
		border: 2px solid map-get($colors, blue);
		position: relative;
		max-width: 319px;

		.skill-percent-circle {
			background-color: map-get($colors, blue);
			border-radius: 50%;
			position: absolute;
			height: 17px;
			top: -8px;
			right: 30px;
			width: 17px;
		}

		.skill-percent-circle-opacity {
			background-color: map-get($colors, blue);
			border-radius: 50%;
			height: 36px;
			opacity: 0.2;
			position: absolute;
			top: -10px;
			right: -10px;
			width: 36px;
		}
	} // opacity: 0.29;
}
</style>
