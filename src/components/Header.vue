<template>
	<header class="header-container">
		<h1>Eduardo Peredo Rivero</h1>
		<h4>Javascript Developer</h4>
	</header>
</template>

<script>
export default {
	name: 'resume-header',
};
</script>

<style lang="scss" scoped>
.header-container {
	background: map-get($colors, blue);
	box-shadow: 0 2px 8px 0 map-get($colors, shadow-black);
	color: map-get($colors, white);
	display: flex;
	flex-direction: column;
	grid-column: 1/3;
	text-align: right;

	h1 {
		font-size: map-get($sizes, very-big);
		letter-spacing: -0.21px;
		margin: 20px 20px 20px 0;
	}

	h4 {
		font-size: map-get($sizes, big);
		letter-spacing: -0.09px;
		margin: 0 20px 20px 0;
	}
}
</style>



