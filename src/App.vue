<template>
	<div id="app">
		<resume-header></resume-header>
		<resume-time-line></resume-time-line>
		<resume-profile></resume-profile>
	</div>
</template>

<script>
import ResumeHeader from './components/Header';
import ResumeTimeLine from './components/TimeLine';
import ResumeProfile from './components/Profile';

export default {
	name: 'app',
	components: {
		ResumeHeader,
		ResumeProfile,
		ResumeTimeLine,
	},
};
</script>

<style lang="scss">
* {
	font-family: 'Roboto', sans-serif;
	font-size: 16px;
}

#app {
	display: grid;
	grid-template-columns: 1fr 1fr;
}
</style>
