<template>
	<div id="app">
		<resume-header></resume-header>
	</div>
</template>

<script>
import ResumeHeader from './components/Header';

export default {
	name: 'app',
	components: {
		ResumeHeader,
	},
};
</script>

<style lang="scss">
* {
	font-family: 'Roboto', sans-serif;
	font-size: 16px;
}
</style>
