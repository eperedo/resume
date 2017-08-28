<template>
	<section class="profile-avatar">
		<figure class="image-container">
			<img class="image-avatar" v-bind:src="urlImage" alt="Eduardo Peredo" />
			<figcaption>
				Developer with 8 years of experience who loves writes javascript for building web applications. I can work in frontend or backend developer using NodeJs.
			</figcaption>
		</figure>
	</section>
</template>

<script>

function data() {
	return {
		urlImage: 'https://avatars1.githubusercontent.com/u/461124?v=4&s=460',
	};
}

export default {
	name: 'profile-avatar',
	data,
};
</script>

<style lang="scss" scoped>
.profile-avatar {
	margin-top: 55px;
}

.image-container {
	align-items: center;
	display: flex;
	flex-direction: column;

	.image-avatar {
		border-radius: 50%;
		height: 250px;
		width: 250px;
	}

	figcaption {
		color: map-get($colors, grey);
		font-size: map-get($sizes, medium);
		height: 124px;
		letter-spacing: 0;
		line-height: 30px;
		margin-top: 20px;
		width: 309px;
	}
}
</style>


