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
	background: #256FE4;
	box-shadow: 0 2px 8px 0 rgba(0, 0, 0, 0.50);
	color: #fff;
	display: flex;
	flex-direction: column;
	text-align: right;

	h1 {
		font-size: 3em;
		letter-spacing: -0.21px;
		margin: 20px 20px 20px 0;
	}

	h4 {
		font-size: 1.125em;
		letter-spacing: -0.09px;
		margin: 0 20px 20px 0;
	}
}
</style>



