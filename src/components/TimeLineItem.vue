<template>
	<section class="time-line-item">
		<div class="time-line-item-date">
			<p class="number">{{item.duration.number}}</p>
			<p class="time">{{item.duration.type}}</p>
		</div>
		<div class="time-line-item-content">
			<p class="title">{{item.companyName}}</p>
			<p class="position">{{item.position}}</p>
			<ul class="jobs">
				<li v-for="text in item.jobs" v-bind:key="text">
					{{text}}
				</li>
			</ul>
		</div>
	</section>
</template>

<script>
export default {
	name: 'time-line-item',
	props: {
		item: {
			type: Object,
			required: true,
		},
	},
};
</script>

<style lang="scss" scoped>
.time-line-item {
	color: map-get($colors, white);
	display: flex;
	font-family: map-get($fonts, black);
	margin-bottom: 5%;

	.time-line-item-content {
		color: map-get($colors, black);
		padding-left: 7%;
		max-width: 70%;

		.title {
			font-family: map-get($fonts, light);
			font-size: map-get($sizes, large);
			margin-top: 1%;
		}

		.position {
			font-family: map-get($fonts, black);
			font-size: map-get($sizes, medium);
		}

		.jobs>li {
			font-family: map-get($fonts, medium);
			font-size: map-get($sizes, small);
			line-height: 19px;
			margin-bottom: 3%;
		}
	}

	.time-line-item-date {
		background-color: map-get($colors, blue);
		box-shadow: 0 2px 8px 0 rgba(0, 0, 0, 0.50);
		height: 109px;
		text-align: center;
		width: 109px;

		.number {
			font-size: map-get($sizes, big);
			margin: 0;
			padding-top: 10%;
		}

		.time {
			font-size: map-get($sizes, medium);
		}
	}
}
</style>


